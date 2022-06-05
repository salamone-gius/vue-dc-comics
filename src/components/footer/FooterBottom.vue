<template>
  <footer class="footer-bottom">
    <div class="container">
        <button class="footer-bt button">sign-up now!</button>
        <nav class="footer-nav">
          <span>follow us</span>
          <ul>
              <li>
                  <a href="#">
                    <img src="../../assets/img/footer-facebook.png" alt="">
                  </a>
              </li>
              <li>
                  <a href="#">
                    <img src="../../assets/img/footer-twitter.png" alt="">
                  </a>
              </li>
              <li>
                  <a href="#">
                    <img src="../../assets/img/footer-youtube.png" alt="">
                  </a>
              </li>
              <li>
                  <a href="#">
                    <img src="../../assets/img/footer-periscope.png" alt="">
                  </a>
              </li>
              <li>
                  <a href="#">
                    <img src="../../assets/img/footer-pinterest.png" alt="">
                  </a>
              </li>
          </ul>
        </nav>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'FooterBottom',
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/mixins.scss';

.footer-bottom {
  background-color: var(--tertiary-color);
  padding: 1rem;

  .container {
    @include flexCenter;
    
    .footer-bt.button {
      background-color: transparent;
      color: var(--primary-color);
      text-transform: uppercase;
      padding: .9375rem;
      border: .1875rem solid var(--secondary-color);
    }

    .footer-bt.button:hover {
      cursor: pointer;
    }

    .footer-bt.button:active {
      transform: translateY(.0625rem);
    }

    .footer-nav {
      display: flex;
      align-items: center;

        span {
          text-transform: uppercase;
          color: var(--secondary-color);
          font-weight: bold;
          margin-right: .9375rem;
        }

        ul li{
          @include sterileLi;

          a {
            text-decoration: none;
          }
        }
    }
  }
}

</style>