<script >

import AppFooter from './components/AppFooter.vue'
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import Hero from './components/Hero.vue'



export default {
  components: {
    AppFooter,
    AppHeader,
    AppMain,
    Hero,
  }
}
</script>

<template>
  <AppHeader />
  <Hero />
  <AppMain />
  <AppFooter />
</template>


<style lang="scss">
@use './style/general.scss';
</style>

