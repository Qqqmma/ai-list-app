<template>
<div id="app">

  <nav>
    <header-component @search-header="lert"/>
    <!-- <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> -->
  </nav>
  <router-view/>

  <footer-component/>
</div>
</template>

<script>
import FooterComponent from './components/FooterComponent.vue';
import HeaderComponent from './components/HeaderModule/HeaderComponent.vue';

export default {
  components: { 
    HeaderComponent,
    FooterComponent,
   },methods: {lert() {alert('hat')}}
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

.container-1200{
  margin: 0 auto;
  padding: 0 15px;
  width: 1200px;
}
</style>
