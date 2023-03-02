<script >

import AppFooter from './components/AppFooter.vue'
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppSidebar from './components/AppSidebar.vue'
import Hero from './components/Hero.vue'



export default {
  components: {
    AppFooter,
    AppHeader,
    AppMain,
    AppSidebar,
    Hero,
  }
}
</script>

<template>
  <AppHeader />
  <Hero />
  <AppMain />
  <AppSidebar />
  <AppFooter />
</template>


<style lang="scss">
@use './style/general.scss';
</style>

