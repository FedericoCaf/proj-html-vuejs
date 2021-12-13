<template>
  <header class="container">
    <div class="row d-flex">

      <div class="logo-header col-2 d-flex align-items-center">
        <img src="../assets/img/avada-marketing-logo.png" alt="logo">
      </div>
      <ul class="d-flex align-items-center justify-content-between col-6">

       <li> <a href=""> ciao </a> <i class="fas fa-chevron-down"></i> </li>
       <li> <a href=""> ciao </a> <i class="fas fa-chevron-down"></i></li>
       <li> <a href=""> ciao </a> </li>
       <li> <a href=""> ciao </a> </li>
       <li> <a href=""> ciao </a> </li>
       <li> <a href=""> ciao </a> </li>
      
     
      </ul>
      <div class="phone-contact col-4 d-flex justify-content-around align-items-center">
         <a href="#"> <i class="fas fa-phone-alt"> <span> (555) 802-1234 </span> </i></a> 
         <button>ciao</button>
      </div>

    </div>
  

  </header>
</template>

<script>

export default {
  name: 'Header'
}


</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';

 header{
   height: 70px;
   background-color: aqua;
     .logo-header{
       height: 70px;
        img{
          width: 100%;
          padding-top: 4px;
          cursor:pointer;
        }
     }
     .phone-contact{
       height: 70px;
        button{
          height: 50%;
          width: 150px;
          border: none;
          border-radius: 5px;
          background-color: lighten( $primary-color, 35% );
          color: $primary-color;
        }
        .fa-phone-alt{
          color: $primary-color;
           span{
             padding-left: 5px;
             color: black;
             font-weight: 400;
           }
        }
     }

     ul{
      //  background-color: crimson;
       height: 70px;
         li{
           height: 35px;
           line-height: 35px;
           border-bottom: 2px solid transparent;
             a{
               text-decoration: none;
               color: black;
             }
             
             .fa-chevron-down{
               font-size: 12px;
               cursor: pointer;
             }
         }

         li:hover{
           border-bottom: 2px solid $primary-color;
         }

         li:hover a, li:hover i{
           color: $primary-color;
         }
      }
 }

</style>