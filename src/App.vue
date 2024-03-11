<script >

import AppNav from './components/AppNav.vue'

import AppCourses from './components/AppCourses.vue'

import AppStatistics from './components/AppStatistics.vue'

import AppSubscribe from './components/AppSubscribe.vue'

import AppFooter from './components/AppFooter.vue'

export default {
  components:{
    AppNav,
    AppCourses,
    AppStatistics,
    AppSubscribe,
    AppFooter,
  }
}
</script>

<template>
  <AppNav></AppNav>
  <AppCourses></AppCourses>
  <AppStatistics></AppStatistics>
  <AppSubscribe></AppSubscribe>
  <AppFooter></AppFooter>
</template>

<style >

</style>
