<template>
 <div class="div">


  <Header/>

  <Jumbosection/>


 </div>


  

</template>

<script>

import Header from './components/Header.vue';
import Jumbosection from './components/Jumbosection.vue';

export default {
  name: 'App',

  components: {
    Header,
    Jumbosection
  }
}
</script>

<style lang="scss">

@import './assets/style/vars.scss';
@import './assets/style/generals.scss'

</style>
