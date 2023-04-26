<template>
  <div class="download-more-button">

    <button class="more-button" @click="$emit('clickMoreButton')">More</button>

  </div>
</template>


<script>
export default {
  
}
</script>


<style scoped>
.download-more-button{
  margin-top: 50px;
  margin-bottom: 50px;
  text-align: center;
}
.more-button{
  cursor: pointer;
  font-size: 16px;
  font-weight: 700;
  padding: 10px 20px;
  border: 1px solid #ff6fd4;
  border-radius: 3px;
  background-color: #f9cdff;
}
</style>