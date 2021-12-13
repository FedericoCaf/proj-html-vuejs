<template>
 <div class="div">


  <Header/>

  <Jumbosection/>

  <Svgsection/>


 </div>


  

</template>

<script>

import Header from './components/Header.vue';
import Jumbosection from './components/Jumbosection.vue';
import Svgsection from './components/Svgsection.vue';

export default {
  name: 'App',

  components: {
    Header,
    Jumbosection,
    Svgsection
  }
}
</script>

<style lang="scss">

@import './assets/style/vars.scss';
@import './assets/style/generals.scss'

</style>
