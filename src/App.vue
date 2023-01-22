<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppSpecial from './components/AppSpecial.vue';
export default {
  name: 'ViteComics',
  components: { AppHeader, AppMain, AppFooter, AppSpecial }
}

</script>

<template>
  <app-header></app-header>
  <app-main></app-main>
  <app-special></app-special>
  <app-footer></app-footer>

</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>