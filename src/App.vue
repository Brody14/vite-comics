<script >

import AppFooter from './components/AppFooter.vue'
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'

export default {
  components: {
    AppFooter,
    AppHeader,
    AppMain,
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

a {
  text-decoration: none;
  color: currentColor;
}

img {
  max-width: 100%;
}

ul,
ol,
menu {
  list-style: none;
}

.container {
  max-width: 900px;
  margin: 0 auto;
  display: flex;
  /* border: 2px solid black; */
}
</style>
