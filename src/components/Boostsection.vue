<template>
<div class="container-global-boost bg-light">
  <div class="container">
     <div class="row d-flex">
       <div class="col-6 text-boost">
         <h1>We Boost Our Clients’ Bottom Line by Optimizing Their Growth Potential.</h1>
         <p>Quisque aliquet, libero consequat elementum convallis, erat risus imperdiet pellentesque sem neque eget.</p>
         <button class="fc-button-orange">Why Work With Us</button>
       </div>
       <div class="col-6 img-boost">
         <img src="../assets/img/we-boost-our-clients-600x549.jpg" alt="img-work">
       </div>
     </div>

     <div class="row d-flex boost-bottom-content">
       <div class="col-6">

         <h3>We Build Relationships</h3>
         <p class="boost-paragraph">Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus maximus nec ut leo. Integer consectetur.</p>

         <h3>Proprietary Processes</h3>
         <p class="boost-paragraph">Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus maximus nec ut leo. Integer consectetur.</p>

       </div>
       <div class="col-6">

         <div class="boost-bottom-right d-flex">
           <div class="fc-icon d-flex justify-content-center align-items-center">
             <i class="fas fa-file-invoice"></i>
           </div>
           <div class="fc-text d-flex flex-column justify-content-between">
             <h4>Accountability</h4>
             <p class="boost-paragraph-right">Curabitur ac leo nunc vestibulum</p>
           </div>       
         </div>
         <div class="boost-bottom-right d-flex">
           <div class="fc-icon d-flex justify-content-center align-items-center">
              <i class="fab fa-leanpub"></i>
           </div>
           <div class="fc-text d-flex flex-column justify-content-between">
             <h4>Transparency</h4>
             <p class="boost-paragraph-right">Curabitur ac leo nunc vestibulum</p>
           </div>       
         </div>
         <div class="boost-bottom-right d-flex">
           <div class="fc-icon d-flex justify-content-center align-items-center">
             <i class="fas fa-chart-line"></i>
           </div>
           <div class="fc-text d-flex flex-column justify-content-between">
             <h4>Investment</h4>
             <p class="boost-paragraph-right">Curabitur ac leo nunc vestibulum</p>
           </div>       
         </div>

       </div>
     </div>

     <div class="awards-title text-center">
       <h2>Awards</h2>
     </div>
     
     <div class="row fc-awards">
       <div class="col-3 text-center">
          <div class="awards-img">
             <img src="../assets/img/award-a-200x191.png" alt="award-a">
          </div>
          <p>Winner Seo Master MAGT</p>
          <p>Smart Start Award 2017</p>     
       </div>
       <div class="col-3 text-center">
          <div class="awards-img">
             <img src="../assets/img/award-a-200x191.png" alt="award-a">
          </div>
          <p>Winner Seo Master MAGT</p>
          <p>Smart Start Award 2017</p>     
       </div>
       <div class="col-3 text-center">
          <div class="awards-img">
             <img src="../assets/img/award-a-200x191.png" alt="award-a">
          </div>
          <p>Winner Seo Master MAGT</p>
          <p>Smart Start Award 2017</p>     
       </div>
       <div class="col-3 text-center">
          <div class="awards-img">
             <img src="../assets/img/award-a-200x191.png" alt="award-a">
          </div>
          <p>Winner Seo Master MAGT</p>
          <p>Smart Start Award 2017</p>     
       </div>
     
     </div>
      

    </div>
  </div>
</template>

<script>
export default {
 name: 'Boostsection'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';

.container-global-boost{
  margin-top: 150px;
  padding: 100px 0;
}

.text-boost{
  margin-top: 50px;
  padding-right: 90px;
  h1{
    font-size: 55px;
    font-weight: 700;
  }
  .fc-button-orange{
    width: 200px;
    padding: 15px;
    font-size: 17px;
  }
}

.img-boost{
  img{
    width: 100%;
    border-radius: 5px;
  }
}

.boost-bottom-content{
  padding-right: 20px;
  margin-top: 120px;
   h3{
     font-size: 33px;
     font-weight: 500;
   }
   .boost-paragraph{
     font-size: 20px;
     margin-bottom: 80px;
   }
}

.boost-bottom-right{
  padding-left: 30px;
  margin-bottom: 50px;
  .fc-icon{
    width: 80px;
    height: 80px;
    border: 2px solid $primary-color;
    border-radius: 20px;
     i{
       font-size: 25px;
       color: $primary-color;
     }
  }

  .fc-text{
    padding-left: 25px;
    .boost-paragraph-right{
      margin-bottom: 0 !important;
      font-size: 17px;
    }
  }
}

.awards-img{
  height: 150px;
   img{
     height: 100%;
   }
}

.awards-title{
  margin-top: 100px;
}

.fc-awards{
  margin-top: 70px;
}

</style>