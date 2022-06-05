<template>
  <div id="app">
    <BaseHeader/>
    <BaseMain/>
    <FooterTop/>
    <FooterMiddle/>
    <FooterBottom/>
  </div>
</template>

<script>
import BaseHeader from './components/header/BaseHeader.vue';
import BaseMain from './components/main/BaseMain.vue';
import FooterTop from './components/footer/FooterTop.vue';
import FooterMiddle from './components/footer/FooterMiddle.vue';
import FooterBottom from './components/footer/FooterBottom.vue';

export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseMain,
    FooterTop,
    FooterMiddle,
    FooterBottom,
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
</style>
