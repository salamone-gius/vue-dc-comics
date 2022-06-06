<template>
  <div class="card">
      <img :src="image" :alt="title">
      <h5>{{title}}</h5>
  </div>
</template>

<script>
export default {
    name: 'BaseCard',
    props: {
        image: String,
        title: String,
    }
}
</script>

<style lang="scss" scoped>

.card {
    width: 10rem;
    margin: 1rem 0.5rem;
    display: inline-block;
    
    img {
        height: 10rem;
    }

    h5 {
        font-size: 1rem;
        margin: 0.5rem 0;
    }
}
</style>