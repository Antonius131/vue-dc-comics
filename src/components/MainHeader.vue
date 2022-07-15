<template>
  <header>
      <nav>
         <div id="logo">
            <img src="../assets/img/dc-logo.png" alt="DC logo">
         </div>
         <div id="nav-menu">
            <ul>
               <li v-for="(link, index) in navMenuItems"
                   :key="index">
                   <a :href="link.link">{{ link.text }}</a>
               </li>
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

<style scoped>
   nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem;
   }

   #logo img {
      height: 60px;
   }

   ul {
      list-style: none;
   }

   ul li {
      display: inline-block;
      padding: .8rem;
      font-size: .75rem;
      text-transform: uppercase;
      font-weight: 600;
   }

   #nav-menu a {
      text-decoration: none;
      color: #212112;
   }
</style>