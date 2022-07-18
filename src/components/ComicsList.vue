<template>
   <div class="card">
      <div class="comic-front">
         <img :src="comicThumb" :alt="comicSeries">
      </div>
      <h4>
         {{ comicSeries }}
      </h4>
   </div>
</template>

<script>
export default {
   props: {
      'comicThumb': String,
      'comicSeries': String
   }
}
</script>

<style>

</style>