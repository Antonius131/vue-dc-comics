<template>
  <footer>
    <div class="container">
      <div id="footer-nav">
        <nav id="nav-items-block">
          <div class="item-block">
            <div class="item">
              <h3>DC Comics</h3>
              <ul>
                <li v-for="(link, index) in dcComicsMenu"
                    :key="index">
                  <a :href="link.link">{{ link.text }}</a>
                </li>
              </ul>
            </div>
            <div class="item">
              <h3>Shop</h3>
              <ul>
                <li v-for="(link, index) in dcShopMenu"
                    :key="index">
                  <a :href="link.link">{{ link.text }}</a>
                </li>
              </ul>
            </div> 
          </div>
          <div class="item-block">
            <h3>DC</h3>
            <ul>
              <li></li>
            </ul>
          </div>
        </nav>
        
        <div>
       </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data: function() {
    return {
      dcComicsMenu: [
        {
            text: 'characters',
            link: '#' 
        },
        {
            text: 'comics',
            link: '#',
        },
        {
            text: 'movies',
            link: '#' 
        },
        {
            text: 'tv',
            link: '#' 
        },
        {
            text: 'games',
            link: '#' 
        },
        {
            text: 'videos',
            link: '#' 
        },
        {
            text: 'news',
            link: '#' 
        }
      ],
      dcShopMenu: [
        {
          text: 'Shop DC',
          link: '#'
        },
        {
          text: 'Shop DC Collectibles',
          link: '#'
        }
      ]
    }
  }
}
</script>

<style scoped>
  footer {
    padding: 2rem 0rem;
    background-image: url(../assets/img/footer-bg.jpg);
    color: #fff;
  }

  #footer-nav {
    display: flex;
    align-content: space-between;
    align-items: center;
  }
</style>