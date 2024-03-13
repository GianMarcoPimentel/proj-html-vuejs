<script >

import AppNav from './components/AppNav.vue'

import AppCourses from './components/AppCourses.vue'

import AppTutoring from './components/AppTutoring.vue'

import AppStatistics from './components/AppStatistics.vue'

import AppStart from './components/AppStart.vue'

import AppBlog from './components/AppBlog.vue'

import AppSubscribe from './components/AppSubscribe.vue'

import AppFooter from './components/AppFooter.vue'

import AppHeader from './components/AppHeader.vue'

export default {
  components:{
    AppNav,
    AppHeader,
    AppCourses,
    AppTutoring, 
    AppStart,
    AppStatistics,
    AppBlog,
    AppSubscribe,
    AppFooter,
  }
}
</script>

<template>
  <AppNav></AppNav>
  <AppHeader></AppHeader>
  <AppCourses></AppCourses>
  <AppTutoring></AppTutoring>
  <AppStart></AppStart>
  <AppStatistics></AppStatistics>
  <AppBlog></AppBlog>
  <AppSubscribe></AppSubscribe>
  <AppFooter></AppFooter>

  <button> <i class="fa-solid fa-arrow-up"></i></button>

  <div class="carrello">

    <i class="fa-solid fa-triangle"></i>
    <i class="fa-solid fa-life-ring"></i>
    <i class="fa-solid fa-book"></i>
    <i class="fa-solid fa-cart-shopping"></i>

  </div>
</template>

<style scoped>
button{
  width: 60px;
  height: 60px;
  border: none;
  border-radius: 50%;
  background-color: #20ad96;
  color: white;


  position: fixed;
  bottom: 20px;
  right: 20px;

  i{
    font-size: 20px;
  }
}
.carrello{
  display: flex;
  flex-flow: column;
  align-items: center;
  gap: 10px;
  fill: inherit;
  padding: 5px;
  border: lightgray solid 1px;
  border-top-left-radius: 5px;
  border-bottom-left-radius: 5px;


  position:fixed;
  top: 100px;
  right: 0px;
}
</style>
