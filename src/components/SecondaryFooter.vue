<template>
  <div class="secondary-footer">
    <div class="container">
      <nav>
          <div id="logo">
            <button type="button" class="btn">Sign up now</button>
          </div>
          <div id="nav-menu">
            <ul>
              <li>
                <h3>Follow us</h3>
              </li>
              <li>
                <img src="../assets/img/footer-facebook.png" alt="Facebook ico">
              </li>
              <li>
                <img src="../assets/img/footer-twitter.png" alt="Twitter ico">
              </li>
              <li>
                <img src="../assets/img/footer-youtube.png" alt="YouTube ico">
              </li>
              <li>
                <img src="../assets/img/footer-pinterest.png" alt="Pinterest ico">
              </li>
              <li>
                <img src="../assets/img/footer-periscope.png" alt="Periscope ico">
              </li>
            </ul>
          </div>
      </nav>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
  .secondary-footer {
    background-color: #303030;
    padding: .5rem 0rem;
  }

  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 0rem;
  }
</style>