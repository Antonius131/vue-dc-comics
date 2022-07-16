<template>
  <div class="secondary-footer">
    <div class="container">
      <nav>
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
                <img :src="imagePath(index)" :alt="icon.alt">
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
          fileName: 'footer-facebook.png',
          alt: 'Facebook ico',
          link: '#',
          path: '/assets/img/'
        },
        {
          fileName: 'footer-twitter.png',
          alt: 'Twitter ico',
          link: '#',
          path: '/assets/img/'
        },
        {
          fileName: 'footer-youtube.png',
          alt: 'YouTUbe ico',
          link: '#',
          path: '/assets/img/'
        },
        {
          fileName: 'footer-pinterest.png',
          alt: 'Pinterest ico',
          link: '#',
          path: '/assets/img/'
        },
        {
          fileName: 'footer-periscope.png',
          alt: 'Periscope ico',
          link: '#',
          path: '/assets/img/'
        }
      ]
    }
  },

  methods: {
    imagePath(index) {
      const path = this.socialIcons[index].path;
      const fileName = this.socialIcons[index].fileName;

      return `${path}${fileName}`;
    }
  }
}
</script>

<style scoped>
  .secondary-footer {
    background-color: #303030;
    padding: 1.5rem 0rem;
  }

  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .d-flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  ul {
    list-style: none;
  }

  h4 {
    color: #3682F9;
  }

  ul li {
    display: inline-block;
    margin: 0rem .5rem;
    text-transform: uppercase;
    font-weight: 600;
  }

  ul img {
  height: 1.5rem;
  }

  button.btn {
    padding: .5rem;
    background-color: transparent;
    border: 2px solid #3682F9;
    color: #fff;
    text-transform: uppercase;
  }
</style>