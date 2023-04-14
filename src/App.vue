<script>
import SiteHeader from './components/SiteHeader.vue';
import SiteFooter from './components/SiteFooter.vue';
import SiteMain from './components/SiteMain.vue';


export default{
  data(){
    return{
      
    }
  },
  components: {
    SiteHeader,
    SiteFooter,
    SiteMain,
  }
}

</script>

<template>
  
 <SiteHeader></SiteHeader>
 
 <SiteMain></SiteMain>

 <SiteFooter></SiteFooter>

</template>

<style>

</style>
