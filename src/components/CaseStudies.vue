<template>

  <div class="container case-studies-container">
    <div class="title-container text-center">
        <h1>Trusted by Leading Organizations</h1>
    </div>


     <div class="container-cases d-flex justify-content-between">

       <div class="inner-container-case">
          <div class="img-cases">
           <img src="../assets/img/case-studies-1-400x450.jpg" alt="case1-img">
          </div>
          <h3>How Spaces attracted five million visitors by improving the content</h3>
          <h2>200%</h2>
          <p>Higher revenue from digital</p>
       </div>
       <div class="inner-container-case">
          <div class="img-cases">
           <img src="../assets/img/case-studies-4-400x450.jpg" alt="case1-img">
          </div>
          <h3>Creativity helped Hemisferio to increase their brand reach vertically</h3>
          <h2>10x</h2>
          <p>Sales increase with the same ad spend</p>
       </div>
       <div class="inner-container-case">
          <div class="img-cases">
           <img src="../assets/img/case-studies-6-400x450.jpg" alt="case1-img">
          </div>
          <h3>How DigitalBox used AI-powered data insight to boost sales</h3>
          <h2>3-year</h2>
          <p>Partnership with Avada Consultant</p>
       </div>  

     </div>
      
      <div class="button-container text-center">
         <button class="fc-button-orange">Read More Cases Studies</button>
      </div>
    

  </div>
  
</template>

<script>
export default {
 name: 'CaseStudios'
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