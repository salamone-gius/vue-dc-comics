<template>
  <section class="hero">
    <img src="../../assets/img/jumbotron.jpg" alt="Jumbotron">
  </section>
</template>

<script>
export default {
    name: 'JumboTron',
}
</script>

<style lang="scss">
section {

    img {
        width: 100%;
        max-height: 19rem;
        object-fit: cover;
        object-position: top;
    }
}
</style>