<template>
  <div class="component">
  <header class="header-component">
    <div class="container-1200">
      <div class="header-content">

        <h1 class="logo">Catalog</h1>
        <ul class="header-links-list">
          <li class="header-link" @click="$router.push({name: 'home'})">AI</li>
          <li class="header-link" @click="$router.push({name: 'about'})">About Us</li>
        </ul>
        <form @submit.prevent>
          <input type="text" v-model="valueInputSearch" name="search" placeholder="Search" class="header-search-input">
          <button @click="$emit('searchHeader', valueInputSearch)">search</button>
        </form>
        

      </div>
    </div>
  </header>
  <div class="bg-green"></div>
  
  </div>
</template>


<script>
import HeaderDescriptionComponent from './components/HeaderDescriptionComponent.vue';
export default {
  components: {
    HeaderDescriptionComponent,
  },
  data() {
    return {
      valueInputSearch: '',
    }
  }
}
</script>


<style scoped>
.header-link{
  cursor: pointer;
}
.header-component{
  height: 35px;
  width: 100%;
  position: fixed;
  display: flex;
  align-items: center;
  border-bottom: 1px solid #c5c5c5;
  background-color: #f8e6ff;
}
.header-content{
  display: flex;
  justify-content: space-between;
}
.header-links-list{
  display: flex;
  gap: 50px;
}
.bg-green{
  background-color: #ff9191;
}
</style>