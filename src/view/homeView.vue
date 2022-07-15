<template>
  <div >
    <carousel/>
    <main-section/>
    <Footer/>
  </div>
</template>
<script>

import carousel from '@/components/carousel.vue';
import MainSection from "@/components/MainSection.vue";
import Footer from "@/components/Footer.vue";

export default{
  name : 'home',
  components :{
    MainSection,
    carousel,
    Footer
  },
}
</script>