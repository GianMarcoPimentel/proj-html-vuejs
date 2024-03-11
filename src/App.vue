<script >

import AppNav from './components/AppNav.vue'

import AppCourses from './components/AppCourses.vue'

import AppStatistics from './components/AppStatistics.vue'

import AppBlog from './components/AppBlog.vue'

import AppSubscribe from './components/AppSubscribe.vue'

import AppFooter from './components/AppFooter.vue'

export default {
  components:{
    AppNav,
    AppCourses,
    AppStatistics,
    AppBlog,
    AppSubscribe,
    AppFooter,
  }
}
</script>

<template>
  <AppNav></AppNav>
  <AppCourses></AppCourses>
  <AppStatistics></AppStatistics>
  <AppBlog></AppBlog>
  <AppSubscribe></AppSubscribe>
  <AppFooter></AppFooter>
</template>

<style >

</style>
