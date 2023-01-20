<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  name: 'ViteComics',
  components: { AppHeader, AppMain, AppFooter }
}

</script>

<template>
  <app-header></app-header>
  <app-main></app-main>
  <app-footer></app-footer>

</template>

<style lang="scss">
/* Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Generics */
body {
  font-family: 'Open Sans', sans-serif;
  height: 100vh;
}

img {
  max-width: 100%;
  height: auto;
}

a {
  color: black;
  text-decoration: none;

}

/* Utils */
.container {
  margin: 0 auto;
  max-width: 1200px;
}
</style>