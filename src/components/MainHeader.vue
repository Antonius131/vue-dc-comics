<template>
  <header>
   <div class="container">
      <nav>
         <div id="logo">
            <a href="#">
               <img src="../assets/img/dc-logo.png" alt="DC logo">
            </a>
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
   </div>
   <MainJumbotron />
  </header>
</template>

<script>
import MainJumbotron from './MainJumbotron.vue'


export default {
    data: function () {
        return {
            navMenuItems: [
                {
                    text: "characters",
                    link: "#",
                    active: false,
                },
                {
                    text: "comics",
                    link: "#",
                    active: true,
                },
                {
                    text: "movies",
                    link: "#",
                    active: false,
                },
                {
                    text: "tv",
                    link: "#",
                    active: false,
                },
                {
                    text: "games",
                    link: "#",
                    active: false,
                },
                {
                    text: "collectibles",
                    link: "#",
                    active: false,
                },
                {
                    text: "videos",
                    link: "#",
                    active: false,
                },
                {
                    text: "fans",
                    link: "#",
                    active: false,
                },
                {
                    text: "news",
                    link: "#",
                    active: false,
                },
                {
                    text: "shop",
                    link: "#",
                    active: false,
                },
            ]
        };
    },
    components: { MainJumbotron }
}
</script>

<style lang="scss" scoped>
   @import '../css/variables.scss';
   @import '../css/mixins.scss';

   nav {
      @include display-flex-between;
      align-items: center;
      padding: 1rem 0rem;
   }

   #logo img {
      height: 60px;
   }

   ul {
      list-style: none;

      li {
         font-size: $link_size;
         text-transform: $font_uppercase;
         display: inline-block;
         padding: .8rem;
         font-weight: 600;
      }
   }

   #nav-menu a {
      color: $font_primary;
      text-decoration: none;

      &.active {
         color: $brand_primary;
      }

      &:hover {
         color: $brand_secondary;
      }
   }
</style>