<template>
  <footer>
    <div class="container">
      <div id="footer-nav">
        <nav>

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
      footerMenuItems: [
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