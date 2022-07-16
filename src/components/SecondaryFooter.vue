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
          </nav>
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