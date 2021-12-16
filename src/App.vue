<template>
 <div class="div">

  <Header/>

  <Jumbosection/>

  <Svgsection/>

  <Brands/>

  <CaseStudies/>

  <Boostsection/>

  <Marketing/>

  <Footer/>

 </div>

</template>

<script>

import Header from './components/Header.vue';
import Jumbosection from './components/Jumbosection.vue';
import Svgsection from './components/Svgsection.vue';
import Brands from './components/Brands.vue';
import CaseStudies from './components/CaseStudies.vue';
import Boostsection from './components/Boostsection.vue';
import Marketing from './components/Marketing.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',

  components: {
    Header,
    Jumbosection,
    Svgsection,
    Brands,
    CaseStudies,
    Boostsection,
    Marketing,
    Footer
  }
}
</script>

<style lang="scss">

@import './assets/style/vars.scss';
@import './assets/style/generals.scss';

.jumbo-left, .jumbo-right{
    animation: transitionIn 3s;
  }
  
  @keyframes transitionIn {
  
    from {
      transform: translateY(15px);
      filter: opacity(0);
   
    }
  
    to {
      transform: translateY(0);
      filter: opacity(1)
    }
    
  }

</style>
