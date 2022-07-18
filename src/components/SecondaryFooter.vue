<template>
  <div class="secondary-footer">
    <div class="container">
      <nav class="d-flex">
          <div id="logo">
            <button type="button" class="btn">Sign up now!</button>
          </div>
          <nav>
            <ul class="d-flex">
              <li>
                <h4>Follow us</h4>
              </li>
              <li v-for="(icon, index) in socialIcons"
                  :key="index">
                <img :src="require(`../assets/img/${icon.src}`)" :alt="icon.alt">
              </li>
            </ul>
          </nav>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      socialIcons: [
        {
          src: 'footer-facebook.png',
          alt: 'Facebook ico',
          link: '#'
        },
        {
          src: 'footer-twitter.png',
          alt: 'Twitter ico',
          link: '#'
        },
        {
          src: 'footer-youtube.png',
          alt: 'YouTUbe ico',
          link: '#',

        },
        {
          src: 'footer-pinterest.png',
          alt: 'Pinterest ico',
          link: '#'
        },
        {
          src: 'footer-periscope.png',
          alt: 'Periscope ico',
          link: '#'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
 @import '../css/_mixins.scss';
@import '../css/_variables.scss';
  .secondary-footer {
    background-color: $bg_secondary;
    padding: 1.5rem 0rem;
  }
  .d-flex {
    @include display-flex-between;
    align-items: center;
  }

  ul {
    font-size: $link_size;
    color: $font_secondary;
    list-style: none;

    li {
      text-transform: $font_uppercase;
      display: inline-block;
      margin: 0rem .5rem;
      font-weight: 600;
    }
    
    img {
      height: 1.5rem;
    }
  }

  h4 {
    color: $brand_primary;
  }
  button.btn {
    padding: .5rem;
    background-color: transparent;
    border: 2px solid $brand_primary;
    color: #fff;
    text-transform: $font_uppercase;
  }
</style>