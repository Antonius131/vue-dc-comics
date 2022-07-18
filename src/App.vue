<template>
  <div id="app">
    <MainHeader />
    <MainContent />
    <PrimaryFooter />
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue';
import MainContent from './components/MainContent.vue';
import PrimaryFooter from './components/PrimaryFooter.vue';


export default {
  name: 'App',
  components: {
    MainHeader,
    MainContent,
    PrimaryFooter,
  }
}
</script>

<style lang="scss">
  @import 'css/variables.scss';
  @import 'css/mixins.scss';

  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
  }

  .container {
    width: $width_container;
    margin: 0 auto;
  }
</style>
