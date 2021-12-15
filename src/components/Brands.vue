<template>

 <div class="container text-center">
    <h1>Some Brands We Work With</h1>
    <h4>Lorem ipsum dolor, sit amet consectetur adipisicing.</h4>
    <div class="brands-container d-flex justify-content-between">
        <img v-for="(brand, index) in brands" :key="index" 
             :src="brand" alt="logo">
    </div>
    <div class="contact-sandy d-flex justify-content-around align-items-center">
      <div class="sandy-container d-flex align-items-center">
          <div class="sandy-img">
            <img src="../assets/img/marketing-expert-cta.png" alt="sandy">
          </div>
          <div class="sandy-text text-start">
            <h5>Sandy Reiff</h5>
            <h6>Marketing Consultant Expert</h6>
          </div>
      </div>
     
      <p class="subtitle-avada">Drive Leads and Sales with Avada</p>

      <button class="btn-free-quote">(555) 802-1234</button>
    </div> 

 </div>
  
</template>

<script>
export default {
 name: 'Brands',

 data(){
   return{
     brands:[
       require("../assets/img/abstract.png"),
       require("../assets/img/cglobal.png"),
       require("../assets/img/next.png"),
       require("../assets/img/hemisferio.png"),
       require("../assets/img/spaces.png"),
       require("../assets/img/digitalbox.png")
     ]
   }
 }


}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

.container{
  h1{
  margin-top: 100px;
  font-size: 50px;
  font-weight: 700;
 }

 h4{
   font-size: 22px;
   margin: 20px 0 60px 0;
 }

 .contact-sandy{
   margin-top: 200px;
   height: 70px;
   box-shadow: 10px 10px 30px;
   border-radius: 10px;
    .subtitle-avada{
      font-size: 22px;
      margin-bottom: 0 !important;
    }
    .btn-free-quote{
      height: 50px;
    }
    .btn-free-quote:hover{
          background-color: $primary-color;
          color: white;
        }

    .sandy-container{
      height: 100%;
    }

    .sandy-img{
      height: 100%;
       img{
         height: 100%;
         border-radius: 50%;
         padding: 7px;
       }
    }

    .sandy-text{
      margin-left: 5px;
      h5{
         margin-bottom: 0 !important;
      }
      h6{
        color: gray;
      }
    
    }
    
 }


}



</style>