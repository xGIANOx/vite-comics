<script>
import MenuItems from '../assets/data/MenuItems.js';
  export default {
    name: "SiteHeader",
    data() {
      return {
        activeItem: 0,
        MenuItems,
      }
    }
  }
</script>

<template>
    <header>

<nav class="navbar navbar-expand-lg">
<div class="container">

  <div class="nav_left">
    <a class="navbar-brand" href="#">
      <img src="/img/dc-logo.png" alt="">
    </a>
  </div>

  <div class="nav_right" id="navbarSupportedContent">
    <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li v-for="(item, index) in MenuItems" :class="activeItem === index ? 'active' : ''" class="d-flex align-items-center mx-3 h-100" @click="activeItem = index">
          <a :href="item.url" class="text-decoration-none">{{ item.title.toUpperCase() }}</a>
        </li>
    </ul>
  </div>
</div>
</nav>

</header>
</template>


<style scoped>

</style>