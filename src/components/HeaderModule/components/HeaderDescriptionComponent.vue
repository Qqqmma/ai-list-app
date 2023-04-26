<template>
  <div class="header-desc-component">

    <h1 class="header-desc-title">Any title</h1>
    <p class="desc-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus fugiat laudantium adipisci voluptate perferendis ut voluptates at? Dolore aspernatur aut fugiat voluptatem quam, perspiciatis dolorem provident necessitatibus odio rerum esse?</p>
    <p>Найти по сфере применения</p>
    <select>
      <option value="copyriting">Копирайтинг</option>
      <option value="chatBot">Чат бот</option>
      <option value="marceting">Маркетинг</option>
    </select>
  </div>
</template>


<script>
export default {
  
}
</script>


<style scoped>
.desc-text{
  margin-bottom: 30px;
}
.header-desc-component{
  padding: 50px 0 50px;
}
h1{
  margin-bottom: 30px;
  font-size: 30px;
  font-weight: 700;
}
</style>