<script>
  export default {
    name: "CardElement",
    props: {
      img: String,
      title: String,
    }
  }
</script>

<template>
  <div class="flex-column">
    <img :src="img" :alt="title + 'Image'">
    <h5>{{ title }}</h5>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables" as *;
  img {
    width: 170px;
    height: 200px;
    margin-top: 2rem;
    padding: 0;
  }
  h5 {
    color: $dc_light;
    text-align: left;
    font-weight: 400;
    font-size: medium;
    margin: 0.5rem 0 2rem;
    text-transform: uppercase; 
  }
</style>