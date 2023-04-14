<script>
import DcThumbs from '../assets/data/DcThumbs.js';
import CardElement from './CardElement.vue';
  export default {
    name: "SiteMain",
    data() {
      return {
        DcThumbs: DcThumbs,
      }
    },
    components:{
        CardElement
    }
  }
</script>

<template>
    <main>
  <div class="jumbotron position-relative">
    <div class="container">
    <div class="row">
      <div class="col d-flex flex-colums">
        <div class="p-2 px-4 position-absolute current_series">CURRENT SERIES</div>
      </div>
    </div>
  </div>
  </div>
  <div>
    <div class="container mt-5 pb-3">
    <div class="row justify-content-center">
        <div class="d-flex flex-wrap">
             <CardElement class="card_element col-2 d-flex" v-for="item in DcThumbs" :img="item.thumb" :title="item.series"></CardElement>
        </div>
      <button class="mt-3 mb-0 py-2 px-5 current_series text-light border-0 load_more">LOAD MORE</button>
      
    </div>
  </div>
  </div>
 </main>
</template>


<style scoped>

</style>