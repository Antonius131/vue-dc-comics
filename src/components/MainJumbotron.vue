<template>
  <div class="jumbotron">
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
   @import '../css/mixins.scss';

   .jumbotron {
      @include background-image('../assets/img/jumbotron.jpg');
      background-position: top;
      height: 300px
   }
</style>