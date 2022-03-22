<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <MyPromotions/>

  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import MyPromotions from './components/MyPromotions.vue'



export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyPromotions,
  }
}
</script>

<style lang="scss">
@import './assets/_style.scss';
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  // -webkit-font-smoothing: antialiased;
  // -moz-osx-font-smoothing: grayscale;
  
}
</style>
