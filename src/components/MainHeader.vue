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
                   <a :href="link.link" :class="{'active' : link.active}">{{ link.text }}</a>
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
               active: false, 
            },
            {
               text: 'comics',
               link: '#',
               active: true, 
            },
            {
               text: 'movies',
               link: '#',
               active: false, 
            },
            {
               text: 'tv',
               link: '#',
               active: false, 
            },
            {
               text: 'games',
               link: '#',
               active: false, 
            },
            {
               text: 'collectibles',
               link: '#',
               active: false, 
            },
            {
               text: 'videos',
               link: '#',
               active: false, 
            },
            {
               text: 'fans',
               link: '#',
               active: false, 
            },
            {
               text: 'news',
               link: '#',
               active: false, 
            },
            {
               text: 'shop',
               link: '#',
               active: false, 
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

   #nav-menu a.active {
      color: #3682F9;
   }
</style>