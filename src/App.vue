<template>
  <div id="app">
    <img src="./assets/logo.png">
    <Episode></Episode>
    <!--<router-view/>-->
  </div>
</template>

<script>
  import HelloWorld from '@/components/HelloWorld'
  import Episode from '@/components/Episode'
  import VueAwesomeSwiper from 'vue-awesome-swiper'
  import Vue from 'vue'

  Vue.use(VueAwesomeSwiper)

  require('@/swiper/swiper.css')

  export default {
    name: 'app',
    components: { HelloWorld, Episode }
  }
</script>

<style>
*{
  margin:0;
  padding:0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
