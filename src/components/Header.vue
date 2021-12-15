<template>
  <header class="container">
    <div class="row d-flex justify-content-between">

      <div class="logo-header d-flex align-items-center">
        <img src="../assets/img/avada-marketing-logo.png" alt="logo">
      </div>

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
      //  background-color: crimson;
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

</style>