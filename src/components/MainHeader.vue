<template>
  <header>
      <nav>
         <div id="logo">
            <img src="../assets/img/dc-logo.png" alt="DC logo">
         </div>
         <div id="nav-menu">
            <ul>
            </ul>
         </div>
      </nav>
  </header>
</template>

<script>
export default {
   data: function() {
      return {
         navMenuItems: [
            {
               text: 'characters',
               link: '#', 
            },
            {
               text: 'comics',
               link: '#', 
            },
            {
               text: 'movies',
               link: '#', 
            },
            {
               text: 'tv',
               link: '#', 
            },
            {
               text: 'games',
               link: '#', 
            },
            {
               text: 'collectibles',
               link: '#', 
            },
            {
               text: 'videos',
               link: '#', 
            },
            {
               text: 'fans',
               link: '#', 
            },
            {
               text: 'news',
               link: '#', 
            },
            {
               text: 'shop',
               link: '#', 
            },
         ]
      }
   }
}
</script>

<style>

</style>