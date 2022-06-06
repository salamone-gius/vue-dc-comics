<template>
  <footer class="footer-top">
    <nav class="container">
      <ul>
        <li>
          <a>
            <img src="../../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
            <span>digital comics</span>
          </a>
        </li>
        <li>
          <a>
            <img src="../../assets/img/buy-comics-merchandise.png" alt="DC Merchandise">
            <span>dc merchandise</span>
          </a>
        </li>
        <li>
          <a>
            <img src="../../assets/img/buy-comics-subscriptions.png" alt="Subscription">
            <span>subscription</span>
          </a>
        </li>
        <li>
          <a>
            <img src="../../assets/img/buy-comics-shop-locator.png" alt="Comic Shop Locator">
            <span>comic shop locator</span>
          </a>
        </li>
        <li>
          <a>
            <img src="../../assets/img/buy-dc-power-visa.svg" alt="DC Power Visa">
            <span>dc power visa</span>
          </a>
        </li>
      </ul>
    </nav>
  </footer>
</template>

<script>
export default {
  name: 'FooterTop',
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/mixins.scss';

.footer-top {
  background-color: var(--secondary-color);
  padding: 1.875rem;

  nav ul {
    display: flex;
    align-items: center;
    justify-content: space-evenly;
  }

  nav ul li {
    @include sterileLi;
  }

  nav ul li a {
    text-decoration: none;
    text-transform: uppercase;
    color: var(--primary-color);
    display: flex;
    align-items: center;
    &:hover {
      cursor: pointer;
    }

    img {
      width: 2rem;
      margin-right: .625rem;
    }
  }
}

</style>