<script>
import SiteHeader from './components/SiteHeader.vue';
import SiteFooter from './components/SiteFooter.vue';

export default{
  data(){
    return{
      
    }
  },
  components: {
    SiteHeader,
    SiteFooter,
  }
}

</script>

<template>
 <SiteHeader></SiteHeader>
 

 <main>
  <div class="container">
    <div class="row">
      <div class="col">
        <h3> --Content goes here-- </h3>
      </div>
    </div>
  </div>
 </main>

 <SiteFooter></SiteFooter>

</template>

<style>

</style>
