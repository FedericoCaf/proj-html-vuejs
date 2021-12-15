<template>

  <div class="container case-studies-container">
    <div class="title-container text-center">
        <h1>Trusted by Leading Organizations</h1>
    </div>

     <div class="container-cases d-flex justify-content-between">

       <div v-for="(item, index) in cases" :key="index" 
            class="inner-container-case">
            <div v-if="(index < 3)" class="inside-case">
                <div class="img-cases">
                  <img :src="item.img" :alt="item.comment">
                </div>
                <h3> {{item.title}} </h3>
                <h2> {{item.bigNumber}} </h2>
                <p> {{item.comment}} </p>
            </div>
         
       </div>
     </div>
      
      <div class="button-container text-center">
         <button class="fc-button-orange">Read More Cases Studies</button>
      </div>
    

  </div>
  
</template>

<script>
export default {
 name: 'CaseStudios',

   data(){
   return{
     cases:[
       {
         img: require("../assets/img/case-studies-1-400x450.jpg"),
         title: 'How Spaces attracted five million visitors by improving the content',
         bigNumber: '200%',
         comment: 'Higher revenue from digital'
       },
       {
         img: require("../assets/img/case-studies-4-400x450.jpg"),
         title: 'Creativity helped Hemisferio to increase their brand reach vertically',
         bigNumber: '10x',
         comment: 'Sales increase with the same ad spend'
       },
       {
         img: require("../assets/img/case-studies-6-400x450.jpg"),
         title: 'How DigitalBox used AI-powered data insight to boost sales',
         bigNumber: '3-year',
         comment: 'Partnership with Avada Consultant'
       },
       {
         img: require("../assets/img/case-studies-5-400x450.jpg"),
         title: 'How DigitalBox used AI-powered data insight to boost sales',
         bigNumber: '3-year',
         comment: 'Partnership with Avada Consultant'
       },
     
     ]
   }
 }


}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';

.case-studies-container{
  h1{
    margin-top: 200px;
    margin-bottom: 100px;
    font-weight: 700;
    font-size: 50px;
  }

  .inner-container-case{
    max-width: 400px;
    h3{
      margin-top: 20px;
      font-size: 30px;
    }
    h2{
      margin-top: 20px;
      font-weight: 700;
      font-size: 52px;
    }
  }

  .button-container{
    margin-top: 50px;
  }

  .fc-button-orange{
    width: 270px;
    padding: 10px;
    font-size: 18px;
  }


}

</style>