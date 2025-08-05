<template>
  <MainPage />
</template>

<script setup>
import MainPage from './components/MainPage.vue';

</script>

<style lang="scss">
@import url('./css/global.scss');

@media screen and (min-width: 700px) {

  .mainPage {
    &__background {
      background-image: url('assets/background2.jpg');
    }
  }

  /* .mainPage__button {
    width: 150px;
    height: 35px;
    font-size: 14px;
  }

  .mainPage__credits {
    font-size: 10px;
    letter-spacing: 2px;
  } */
  
}
</style>
