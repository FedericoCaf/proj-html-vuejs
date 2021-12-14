<template>

  <div class="container">
    <div class="row">
      <div class="col-6 svg-container">
        <img src="../assets/svg/img1.svg" alt="svg-img">
      </div>
      <div class="col-6 text-container">
          <h5>
            <i class="fas fa-circle fc-blue"></i> 
            Business Growth
          </h5>
          <h1>Increase Brand Awareness</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime, molestias reiciendis cum, quos in incidunt at temporibus laboriosam exercitationem
          </p>
          <button class="fc-button-orange">Get a consultation</button>
      </div>
    </div>
    <div class="row">
       <div class="col-6 text-container">
         <h5>
            <i class="fas fa-circle fc-yellow"></i> 
            Business Growth
          </h5>
          <h1>Increase Brand Awareness</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime, molestias reiciendis cum, quos in incidunt at temporibus laboriosam exercitationem.
          </p>
          <button class="fc-button-orange">Get a consultation</button>
       </div>
       <div class="col-6 svg-container">
          <img src="../assets/svg/img2.svg" alt="svg-img">
       </div>      
    </div>
    <div class="row">
       <div class="col-6 svg-container">
         <img src="../assets/svg/img3.svg" alt="svg-img">
       </div>
      <div class="col-6 text-container">
         <h5>
            <i class="fas fa-circle fc-green"></i> 
            Business Growth
          </h5>
          <h1>Increase Brand Awareness</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime, molestias reiciendis cum, quos in incidunt at temporibus laboriosam exercitationem.
          </p>
          <button class="fc-button-orange">Get a consultation</button>
      </div>
    </div>

  </div>
  
</template>

<script>
export default {
  name: 'Svgsection'

}

</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

.svg-container{
  height: 600px;
  margin-top: 100px;
  // background-color: lightskyblue;
   img{
     height: 100%;
   }
}

.text-container{
   padding: 100px;
   height: 600px;
   margin-top: 100px;
   h1{
     font-size: 50px;
     font-weight: 700;
   }
    p{
      font-size: 25px;
    }
  
    .fc-button-orange{
      width: 50%;
    }
    .fa-circle.fc-blue{
      color: #0064FE;
    }
    .fa-circle.fc-yellow{
      color: #F8CC23;
    }
    .fa-circle.fc-green{
      color: #3BC77B;
    }
}

</style>