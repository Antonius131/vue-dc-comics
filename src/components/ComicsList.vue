<template>
   <div class="card">
      <div class="comic-front">
         <img :src="comicThumb" :alt="comicSeries">
      </div>
      <div class="comic-caption">
         <h4>
            {{ comicSeries }}
         </h4>
      </div>
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

<style lang="scss" scoped>
@import '../css/_variables.scss';
   .card {
      width: calc((100% / 6) - 0.2rem);
      margin: .1rem;

      .comic-front {
         width: 150px;
         height: 150px;

         img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
         }
      }

      .comic-caption {
         padding: 0.75rem 0;

         h4 {
            text-transform: uppercase;
            font-weight: 100;
            font-size: $link_size;
         }
      }
   }
</style>