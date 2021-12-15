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

       <div v-for="(award, index) in awards" :key="index" class="col-3 text-center">
          <div class="awards-img" :class="award.color">
             <img :src="award.img" :alt="award.award1">
          </div>
          <p> {{award.award1}} </p>
          <p>{{award.award2}} </p>     
       </div>

     
     </div>
      

    </div>
  </div>
</template>

<script>
export default {
 name: 'Boostsection',

   data(){
   return{
     awards:[
       {
         img: require("../assets/img/award-a-200x191.png"),
         award1: 'Winner Seo Master MAGT',
         award2: 'Smart Start Award 2017',
         color: 'color-azure'
       },
       {
         img: require("../assets/img/award-b-200x191.png"),
         award1: 'Top Social Media Agencies',
         award2: 'Next Partner 2018',
         color: 'color-orange'
       },
       {
         img: require("../assets/img/award-c-200x191.png"),
         award1: '10 Fastest Growing Abstract',
         award2: 'Solution Providers 2019',
         color: 'color-red'
       },
       {
         img: require("../assets/img/award-d-200x191.png"),
         award1: 'National Excellence Agencie',
         award2: 'Award Winner 2020',
         color: 'color-blue'
       },
      
     
     ]
   }
 }
 
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
    h4{
      transition: all 0.3s;
      cursor: pointer;
    }
    h4:hover{
      color: $primary-color;
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
   .color-azure{
     filter:hue-rotate(180deg)
   }
   .color-orange{
     filter:hue-rotate(0deg)
   }
   .color-red{
     filter:hue-rotate(340deg)
   }
   .color-blue{
     filter:hue-rotate(210deg)
   }
}

</style>