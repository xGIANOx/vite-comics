<script>
  import SitesBanner from '../assets/data/SitesBanner.js';
  export default {
    name: "SitesBanner",
    data() {
      return {
        SitesBanner,
      }
    }
  }
</script>

<template>
    <div class="pre_footer">
    <div class="container ps-5 pe-5">
      <div class="row">
        <div class="col d-flex align-items-center py-4 justify-content-around">
          <ul class="d-flex">
            <li v-for="site in SitesBanner" class="mx-4 d-flex align-items-center">
                <img height="70" :src="site.img" :alt="site.title.toUpperCase() + ' Image'" class="me-2">
                <a :href="site.link" class="text-light text-decoration-none">{{ site.title.toUpperCase() }}</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
</style>