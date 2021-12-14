<template>
 <div class="div">

  <Header/>

  <Jumbosection/>

  <Svgsection/>

  <Brands/>

  <CaseStudies/>

  <Footer/>


 </div>


  

</template>

<script>

import Header from './components/Header.vue';
import Jumbosection from './components/Jumbosection.vue';
import Svgsection from './components/Svgsection.vue';
import Brands from './components/Brands.vue';
import CaseStudies from './components/CaseStudies.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',

  components: {
    Header,
    Jumbosection,
    Svgsection,
    Brands,
    CaseStudies,
    Footer
  }
}
</script>

<style lang="scss">

@import './assets/style/vars.scss';
@import './assets/style/generals.scss';

</style>
