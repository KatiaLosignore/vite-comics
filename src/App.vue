<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppSpecial from './components/AppSpecial.vue';
export default {
  name: 'ViteComics',
  components: { AppHeader, AppMain, AppFooter, AppSpecial},
  data() {
    return {
      mainCards: [
        {
          thumb:
          "https://static.dc.com/dc/files/default_images/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?w=250",
          price: '$19.99',
          series: 'Action Comics',
          type: 'comic book',
        },
        {
          thumb:
          "https://static.dc.com/dc/files/default_images/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?w=250",
          price: '$3.99',
          series: 'American Vampire 1976',
          type: 'comic book',
        },
        {
          thumb:
          "https://static.dc.com/dc/files/default_images/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?w=250",
          price: '$16.99',
          series: 'Aquaman',
          type: 'graphic novel',
        },
        {
          thumb:
          "https://static.dc.com/dc/files/default_images/batgirl_v5_1_5b23e1f1124941.50950783.jpg?w=250",
          price: '$2.99',
          series: 'Batgirl',
          type: 'comic book',
        },
        {
          thumb:
          "https://static.dc.com/dc/files/default_images/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?w=250",
          price: '$3.99',
          series: 'Batman',
          type: 'comic book',
        },
        {
          thumb:
          "https://static.dc.com/dc/files/default_images/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?w=250",
          price: '$2.99',
          series: 'Batman Beyond',
          type: 'comic book',
        },
        {
          thumb:
          "https://static.dc.com/dc/files/default_images/BMSM_5d4361b7116261.74371456.jpg?w=250",
          price: '$3.99',
          series: 'Batman/Superman',
          type: 'comic book',
        },
        {
          thumb:
          "https://static.dc.com/dc/files/default_images/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?w=250",
          price: '$4.99',
          series: 'Batman/Superman Annual',
          type: 'comic book',
        },
        {
          thumb:
          "https://static.dc.com/dc/files/default_images/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?w=250",
          price: '$5.99',
          series: 'Batman: The Joker War Zone',
          type: 'comic book',
        },
        {
          thumb:
          "https://static.dc.com/dc/files/default_images/cover-v2_5f40314645a734.37285065.png?w=250",
          price: '$6.99',
          series: 'Batman: Three Jokers',
          type: 'comic book',
        },
        {
          thumb:
          "https://static.dc.com/dc/files/default_images/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?w=250",
          price: '$4.99',
          series: 'Batman: White Knight Presents: Harley Quinn',
          type: 'comic book',
        },
        {
          thumb:
          "https://static.dc.com/dc/files/default_images/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?w=250",
          price: '$16.99',
          series: 'Catwoman',
          type: 'graphic novel',
        },
      ],

    }
  }
}

</script>

<template>
  <app-header></app-header>
  <app-main :cards="mainCards"></app-main>
  <app-special></app-special>
  <app-footer></app-footer>

</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>