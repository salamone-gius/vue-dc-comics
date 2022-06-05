<template>
  <footer class="footer-middle">
    <div class="container">
      <div class="footer-md-left">
        <div class="col left">
          <ul>
            <p>DC COMICS</p>
            <li>
              <a href="#">Characters</a>
            </li>
            <li>
              <a href="#">Comics</a>
            </li>
            <li>
              <a href="#">Movies</a>
            </li>
            <li>
              <a href="#">Tv</a>
            </li>
            <li>
              <a href="#">Games</a>
            </li>
            <li>
              <a href="#">Videos</a>
            </li>
            <li>
              <a href="#">News</a>
            </li>
          </ul>
          <ul>
            <p>SHOP</p>
            <li>
              <a href="#">Shop DC</a>
            </li>
            <li>
              <a href="#">Shop DC Collectibles</a>
            </li>
          </ul>
        </div>
        <div class="col middle">
          <ul>
            <p>DC</p>
            <li>
              <a href="#">Terms Of Use</a>
            </li>
            <li>
              <a href="#">Privacy Policy (New)</a>
            </li>
            <li>
              <a href="#">Ad Choices</a>
            </li>
            <li>
              <a href="#">Advertising</a>
            </li>
            <li>
              <a href="#">Jobs</a>
            </li>
            <li>
              <a href="#">Subscriptions</a>
            </li>
            <li>
              <a href="#">Talent Workshops</a>
            </li>
            <li>
              <a href="#">CPSC Certificates</a>
            </li>
            <li>
              <a href="#">Ratings</a>
            </li>
            <li>
              <a href="#">Shop Help</a>
            </li>
            <li>
              <a href="#">Contact us</a>
            </li>
          </ul>
        </div>
        <div class="col right">
          <ul>
            <p>SITES</p>
            <li>
              <a href="#">DC</a>
            </li>
            <li>
              <a href="#">MAD Magazine</a>
            </li>
            <li>
              <a href="#">DC Kids</a>
            </li>
            <li>
              <a href="#">DC Universe</a>
            </li>
            <li>
              <a href="#">DC Power Visa</a>
            </li>
          </ul>
        </div>
      </div>
      <div class="footer-md-right">
        <img src="../../assets/img/dc-logo-bg.png" alt="dc-logo-bg">
      </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'FooterMiddle',
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/mixins.scss';

.footer-middle {
  background-image: url(../../assets/img/footer-bg.jpg);

  .container {
    @include flexCenter;

    .footer-md-left {
      display: flex;

      ul {
        margin: 1rem 1.5rem;
      }

      p {
        color: var(--primary-color);
      }

      li {
        list-style: none;

        a {
        text-decoration: none;
        color: lightgray;
        font-size: .75rem;
        }
      }
    }

    .footer-md-right img {
      width: 16rem;
    }
  }
}

</style>