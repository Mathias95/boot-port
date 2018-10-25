<template>
  <div id="app">
    <main-navigation/>
    <router-view/>
    <main-footer/>
  </div>
</template>

<style lang="scss">
//Import global scss styling
@import "./assets/scss/main";
</style>

<script>
import MainNavigation from '@/components/MainNavigation.vue';
import MainFooter from '@/components/MainFooter.vue';
export default {
    components: {
    MainNavigation,
    MainFooter
  }
}
</script>