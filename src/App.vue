<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <MyPromotions/>
    <MyForum/>
    <MyComunities/>
    <MyNewsletter/>
    <MyFooter/>
    <MySocialFooter/>

  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import MyPromotions from './components/MyPromotions.vue'
import MyForum from './components/MyForum.vue'
import MyComunities from './components/MyComunities.vue'
import MyNewsletter from './components/MyNewsletter.vue'
import MyFooter from './components/MyFooter.vue'
import MySocialFooter from './components/MySocialFooter.vue'



export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyPromotions,
    MyForum,
    MyComunities,
    MyNewsletter,
    MyFooter,
    MySocialFooter,
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
