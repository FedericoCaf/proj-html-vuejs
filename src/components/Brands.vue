<template>

 <div class="container text-center">
    <h1>Some Brands We Work With</h1>
    <h4>Lorem ipsum dolor, sit amet consectetur adipisicing.</h4>
    <div class="brands-container d-flex justify-content-between">
        <img src="../assets/img/abstract.png" alt="logo">
        <img src="../assets/img/cglobal.png" alt="logo">
        <img src="../assets/img/next.png" alt="logo">
        <img src="../assets/img/hemisferio.png" alt="logo">
        <img src="../assets/img/spaces.png" alt="logo">
        <img src="../assets/img/digitalbox.png" alt="logo">
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
 name: 'Brands'
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