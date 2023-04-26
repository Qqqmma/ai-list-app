<template>
  <div class="container-1200">
    <!-- Динамически отрисовываищийся список -->
    <div class="ai-cards-list">
      <div 
        class="ai-card-item"
        v-for="item in renderList"
        :key="item.idKey"
      >
        <img :src="item.logoAI" alt="" class="ai-card-img">
        <div class="ai-card-title">
          <h3>
          {{ item.name + item.idKey}}
          </h3>
        </div>
        <div class="ai-card-task">
          {{ item.taskAI }}
        </div>
        <div class="ai-card-scopes">
          {{ item.scopesOfApplication }}
        </div>
        <div class="ai-card-trunsform">
          {{ item.transformInfo }}
        </div>
        <div class="ai-card-description">
          {{ textReduction(item.description) }}
        </div>
      </div>
    </div>

    <load-component v-if="!loadinAnimateHiden"/>

    <download-more-button @clickMoreButton="addToRenderList"/>
  </div>
</template>


<script>
import DownloadMoreButton from './components/DownloadMoreButton.vue';
import LoadComponent from './components/LoadComponent.vue';

export default {
  components: { 
    DownloadMoreButton,
    LoadComponent,
  },

  props: ["data-base-emulator"],
  data() {
    return {
      renderList: [],
      renderListLength: 9,

      loadinAnimateHiden: true,
    }
  },
  mounted() {
    this.updateRenderList();
  },
  methods: {
    updateRenderList() {
      this.startLoading();
      setTimeout(() => {
        this.renderList = this.dataBaseEmulator.slice(0, this.renderListLength);
        this.loadinAnimateHiden = true;
      }, 1000);
    },
    startLoading() {
      this.loadinAnimateHiden = false;
    },
    addToRenderList() {
      this.renderListLength += 3;
      this.updateRenderList();
      console.log(this.renderListLength);
      console.log(this.renderList);
    },
    textReduction(text) {
      return text.split('').slice(0, 20).join('') + '...';
    },
    searchInDataBase(inputValue) {
      let searchResult = [];
      for (let item of this.DataBaseEmulator){
        if (item.name.includes(inputValue)) searchResult.push(item);
      }
      this.renderList = searchResult;
    }
  },
}
</script>


<style>
.ai-cards-list{
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 40px;
  padding-top: 80px;
}
.ai-card-item{
  border-radius: 10px;
  padding: 10px;
  border: 1px solid #ccc;
  background-color: #f8e6ff;
}
.ai-card-img{
  width: 100%;
}
</style>