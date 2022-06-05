<template>
  <footer class="footer-top">
    <nav class="container">
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a :class="{active : link.current}" :href="link.url">
            <!-- <img :src="link.src" :alt="link.text"> -->
            {{link.text}}
            </a>
        </li>
      </ul>
    </nav>
  </footer>
</template>

<script>
export default {
  name: 'FooterTop',
    data() {
    return {
      links: [
        {
          text: "digital comics",
          url: "#",
          current: false,
          src: '../../assets/img/buy-comics-digital-comics.png',
        },
        {
          text: "dc merchandise",
          url: "#",
          current: true,
          src: '../../assets/img/buy-comics-merchandise.png',
        },
        {
          text: "subscription",
          url: "#",
          current: false,
          src: '../../assets/img/buy-comics-subscriptions.png',
        },
        {
          text: "comic shop locator",
          url: "#",
          current: false,
          src: '../../assets/img/buy-comics-shop-locator.png',
        },
        {
          text: "dc power visa",
          url: "#",
          current: false,
          src: '../../assets/img/buy-dc-power-visa.svg',
        }
      ]
    }
  }
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
  }

}

</style>