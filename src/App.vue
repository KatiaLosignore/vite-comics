<script>
import AppHeader from './components/AppHeader.vue';
export default {
  name: 'ViteComics',
  components: { AppHeader }
}

</script>

<template>
  <app-header></app-header>
  <main></main>
  <footer></footer>

</template>

<style>
/* Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Generics */
body {
  font-family: 'Open Sans', sans-serif;
  min-height: 100vh;
  /* background-image: url('./assets/img/jumbotron.jpg');
  background-position: center;
  background-repeat: no-repeat; */
}

img {
  max-width: 100%;
  height: auto;
}

a {
  color: black;
  text-decoration: none;
  text-transform: uppercase;
}

/* Utils */
.container {
  margin: 0 auto;
  max-width: 1200px;
}
</style>