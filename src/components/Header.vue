<template>
  <header class="container">
    <div class="row d-flex justify-content-between">

      <div class="logo-header d-flex align-items-center">
        <img src="../assets/img/avada-marketing-logo.png" alt="logo">
      </div>

      <ul class="d-flex align-items-center justify-content-between">
        <li> <a href=""> ciao </a> <i class="fas fa-chevron-down"></i> </li>
        <li> <a href=""> ciao </a> <i class="fas fa-chevron-down"></i></li>
        <li> <a href=""> ciao </a> </li>
        <li> <a href=""> ciao </a> </li>
        <li> <a href=""> ciao </a> </li>
        <li> <a href=""> ciao </a> </li>
      </ul>

      <div class="phone-contact d-flex justify-content-around align-items-center">
         <a href="#"> <i class="fas fa-phone-alt"> <span> (555) 802-1234 </span> </i></a> 
         <button class="btn-free-quote">Free Quote</button>
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
   height: 100px;
   font-size: 23px;
     .logo-header{
       height: 100px;
       width: 270px;
        img{
          width: 100%;
          padding-top: 4px;
          cursor:pointer;
        }
     }
     .phone-contact{
       height: 100px;
       width: 400px;
        // .btn-free-quote{
        //   height: 50%;
        //   width: 150px;
        //   border: none;
        //   border-radius: 5px;
        //   background-color: lighten( $primary-color, 35% );
        //   color: $primary-color;
        // }
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
       height: 100px;
       width: calc(100% - 700px);
         li{
          font-size: 23px;
          padding-right: 7px;
           line-height: 35px;
           border-bottom: 2px solid transparent;
             a{
               text-decoration: none;
               color: black;
               padding: 15px;
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