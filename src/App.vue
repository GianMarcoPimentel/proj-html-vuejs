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
</template>

<style >

</style>
