<template>
  <div id="app">
    <div class="lines">
      <div class="container">
        <div class="row">
          <div class="col-line">
            <div class="line"></div>
          </div>
          <div class="col-line">
            <div class="line"></div>
          </div>
          <div class="col-line">
            <div class="line"></div>
          </div>
          <div class="col-line">
            <div class="line"></div>
          </div>
        </div>
      </div>
    </div>
    
    <main-navigation/>
    <router-view/>
  </div>
</template>

<style lang="scss">
//Import global scss styling
@import "./assets/scss/main";
</style>

<script>
import MainNavigation from '@/components/MainNavigation.vue';
export default {
    components: {
    MainNavigation,
  }
}
</script>