<template>
  <footer>
    <div class="container">
      <div class="d-flex">
        <div id="footer-nav">
          <nav id="nav-items-block">
            <div class="item-block">
              <div class="item">
                <h4>DC Comics</h4>
                <ul>
                  <li v-for="(link, index) in dcComicsMenu"
                      :key="index">
                    <a :href="link.link">{{ link.text }}</a>
                  </li>
                </ul>
              </div>
              <div class="item">
                <h4>Shop</h4>
                <ul>
                  <li v-for="(link, index) in dcShopMenu"
                      :key="index">
                    <a :href="link.link">{{ link.text }}</a>
                  </li>
                </ul>
              </div> 
            </div>
            <div class="item-block">
              <div class="item">
                <h4>DC</h4>
                <ul>
                    <li v-for="(link, index) in dcMenu"
                        :key="index">
                      <a :href="link.link">{{ link.text }}</a>
                    </li>
                </ul>
              </div>
            </div>
            <div class="item-block">
              <div class="item">
                <h4>Sites</h4>
                <ul>
                  <li v-for="(link, index) in sitesMenu"
                      :key="index">
                    <a :href="link.link">{{ link.text }}</a>
                  </li>
                </ul>
              </div>
            </div>
          </nav>
          
          <div>
        </div>
        </div>
        <div id="dc-image">
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
      ],
      dcMenu: [
        {
          text: 'Terms Of Use',
          link: '#'
        },
        {
          text: 'Privacy Policy (New)',
          link: '#'
        },
        {
          text: 'Ad Choices',
          link: '#'
        },
        {
          text: 'Advertising',
          link: '#'
        },
        {
          text: 'Jobs',
          link: '#'
        },
        {
          text: 'Subscription',
          link: '#'
        },
        {
          text: 'Talen Workshops',
          link: '#'
        },
        {
          text: 'CPSC Certificates',
          link: '#'
        },
        {
          text: 'Ratings',
          link: '#'
        },
        {
          text: 'Shop Help',
          link: '#'
        },
        {
          text: 'Contact Us',
          link: '#'
        },
      ],
      sitesMenu: [
        {
          text: 'DC',
          link: '#'
        },
        {
          text: 'MAD Magazine',
          link: '#'
        },
        {
          text: 'DC Kids',
          link: '#'
        },
        {
          text: 'DC Universe',
          link: '#'
        },
        {
          text: 'DC Power Visa',
          link: '#'
        }
      ],
    }
  }
}
</script>

<style scoped>
  footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    color: #fff;
  }

  .d-flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  #footer-nav {
    width: 55%;
    padding: 2rem 0rem;
  }

  #nav-items-block {
    display: flex;
    align-content: space-between;
  }

  .item-block {
    margin-right: 1.5rem;
  }

  .item {
    margin-bottom: 1rem;
  }

  .item h4 {
    text-transform: uppercase;
    margin-bottom: .55rem;
  }

  .item ul {
    list-style: none;
    font-size: .75rem;
  }

  .item li {
    padding: .2rem;
  }
  .item a {
    text-decoration: none;
    color: rgba(255,255,255,.5);
  }

  #dc-image {
    width: 45%;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-size: 100%;
    background-repeat: no-repeat;
    background-position: center;
    height: 360px;
  }
</style>