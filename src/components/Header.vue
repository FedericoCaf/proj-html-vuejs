<template>
  <header class="container global-wrapper">
    <div class="fc-hamb text-center">
       <i class="fas fa-bars"></i>
    </div>
    <div class="row d-flex justify-content-between">

      <div class="logo-header d-flex align-items-center">
        <img src="../assets/img/avada-marketing-logo.png" alt="logo">
      </div>

<!-- ciclo gli elementi del menu assegnano al primo la classe active -->
      <ul class="d-flex align-items-center justify-content-between">
        <li :class="{active: index===0}"
         v-for="(item, index) in menu" :key="index">
          <a href="#">
            {{item}}
          </a>
           <i v-if="(index < 2)" class="fas fa-chevron-down"></i>
        </li>
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
  name: 'Header',

 data(){
   return{
     menu:['Home', 'Services', 'Why Us', 'Case Studies', 'About', 'Blog']
   }
 }

}

</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';

.global-wrapper{
  position: relative;
}

 header{
   height: 100px;
   font-size: 20px;
     .logo-header{
       height: 100px;
       width: 270px;
        img{
          width: 100%;
          padding-top: 4px;
          cursor:pointer;
        }
     }

//menu hamburger che si attiva con media query
      .fc-hamb{
        position: absolute;
        display: none;
        cursor: pointer;
        right: 15px;
        top:20px;
        border-radius: 7px;
        font-size: 18px;
        width: 60px;
        height: 60px;
        background-color: white;
        padding-top: 9px;
        box-shadow: 5px 5px 35px -15px;
          i{
            font-size: 35px;
          }
     }
     
     .phone-contact{
       height: 100px;
       width: 400px;
        .btn-free-quote:hover{
          background-color: $primary-color;
          color: white;
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
       height: 100px;
       width: calc(100% - 700px);
       margin-bottom: 0 !important;
         li{
          font-size: 18px;
          padding-right: 8px;
           line-height: 35px;
           border-bottom: 2px solid transparent;
           transition: all 0.5s;
             a{
               text-decoration: none;
               color: black;
               transition: all 0.5s;
              //  padding: 10px;
             }
             
             .fa-chevron-down{
               font-size: 12px;
               cursor: pointer;
             }
         }

         .active{
           border-bottom: 2px solid $primary-color;
         }

         li:hover{
           border-bottom: 2px solid $primary-color;
         }

         li:hover a, li:hover i{
           color: $primary-color;
         }
      }
 }

 @media (max-width:1400px){
   header{
     ul li{
       font-size: 15px;
     }
   }
 }

 @media (max-width:1199px){
 header{
   ul li{
     display: none;
   }
   .phone-contact a{
     display: none;
   }

   .fc-hamb{
     display: block;
   }
  
 }

  
   
 }

</style>