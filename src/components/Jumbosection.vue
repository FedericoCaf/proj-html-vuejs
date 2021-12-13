<template>
  <div class="container-jumbo">
      <div class="container">
        <div class="row inner-container d-flex align-items-center">
            <div class="jumbo-left col-7">
              <h1>Unlock Your Online Growth Potential</h1>
              <h4>Online marketing to secure customer retention, leads, and sales. We focus on the bigger picture.</h4>
              <button>Our Service <i class="fas fa-arrow-right"></i> </button>
            </div>
            <div class="jumbo-right col-5">
               <div class="contact-card">
                 <div class="img-card-top">
                    <img src="../assets/img/marketing-consultant-expert.jpg" alt="consultant">
                 </div>
                    <h5> <strong>Richard Madsen</strong> </h5>
                    <h6>Marketing Consultant Expert</h6>
                    <a href="#"> <i class="fas fa-phone-alt"> <span> (555) 802-1234 </span> </i></a> 

                    <input type="text" placeholder="Your Name*">
                    <input type="text" placeholder="Your Email*">
                    <input type="text" placeholder="Your Phone Number*">
                    <button> Get a Callback </button>
                    <p>By submitting my data I agree to be contacted</p>
    
               </div>
            </div>
        </div>
      </div>
  </div>
</template>

<script>

export default {
 name: 'Jumbosection'
}

</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';

.container-jumbo{
  height: 600px;
  background-image: url('../assets/img/marketing-intro.jpg');
  background-size:cover;
  background-position: center;
  background-color:green;
   .inner-container{
     height: 500px;
   }
}

.jumbo-left{
  height: 300px;
  // background-color: lightpink;
  color: white;
   button{
     border: none;
     border-radius: 5px;
     background-color: white;
     color: black;
     padding: 25px;
     width: 300px;
     font-size: 25px;
      i{
        margin-left: 5px;
      }
   }
   h1{
     font-size: 80px;
     font-weight: 700;
     color: white;
   }
   h4{
     font-size: 35px;
     margin: 30px 0;
   }
}

.jumbo-right{
  height: 300px;
  // background-color:lightslategrey;
}

.contact-card{
  height: 540px;
  width: 390px;
  border-radius: 10px;
  text-align: center;
  padding: 15px;
  background-color:white;
  box-shadow: 10px 10px 30px;
   .fa-phone-alt{
          color: $primary-color;
           span{
             padding-left: 5px;
             color: black;
             font-weight: 400;
           }
        }
   p:last-child{
    font-size: 10px;
    margin-top: 5px;
    color: gray;
    }
    h6{
      color: gray;
    }
   input{
     width: 90%;
     padding: 20px;
     border: 1px solid lightgrey;
     border-radius: 10px;
     margin: 10px;
     outline: none;
   }
   button{
     width: 90%;
     margin-top: 20px;
     padding: 10px;
     border: none;
     border-radius: 25px;
     background-color: $primary-color;
     color: white;
   }
   .img-card-top{
     height: 50px;
     width: 100%;
     margin-bottom: 10px;
      img{
        height: 100%;
        border-radius: 50%;
      }
   }
}

</style>