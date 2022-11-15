<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
export default {
  name: "App",
  components: { AppHeader, AppMain, AppFooter },
};
</script>

<template>
  <app-header />
  <app-main />
  <app-footer />
</template>

<style lang="scss">
@use './style/general'
</style>
