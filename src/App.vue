<script >

import AppFooter from './components/AppFooter.vue'
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppSidebar from './components/AppSidebar.vue'


export default {
  components: {
    AppFooter,
    AppHeader,
    AppMain,
    AppSidebar,
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppSidebar />
  <AppFooter />
</template>


<style lang="scss">
@use './style/general.scss';
</style>

