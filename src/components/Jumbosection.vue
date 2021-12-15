<template>
  <div class="container-jumbo">
    <div class="fc-demos text-center">
       <i class="fas fa-th-list"></i>
       <p>Demos</p>
    </div>
    <div class="fc-on-sale text-center">
       <i> <span> $ </span> 39 </i>
       <p>On Sale</p>
    </div>
 
   
      <div class="container">
        <div class="row inner-container d-flex align-items-center">
            <div class="jumbo-left col-6">
              <h1>Unlock Your Online Growth Potential</h1>
              <h4>Online marketing to secure customer retention, leads, and sales. We focus on the bigger picture.</h4>
              <button class="fc-btn-our-services">Our Services <i class="fas fa-arrow-right"></i> </button>
            </div>
            <div class="jumbo-right col-6">
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
                    <button class="fc-callback"> Get a Callback </button>
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
  position: relative;
  height: 720px;
  margin-bottom: 50px;
  background-image: url('../assets/img/marketing-intro.jpg');
  background-size:cover;
  background-position: center;
  background-color:green;
   .inner-container{
     height: 500px;
   }

   .fc-demos{
     position: absolute;
     cursor: pointer;
     right: 15px;
     top:20px;
     border-radius: 7px;
     font-size: 12px;
     width: 60px;
     height: 60px;
     background-color: white;
     padding-top: 9px;
      i{
        font-size: 25px;
      }
   }
   .fc-on-sale{
     position: absolute;
     cursor: pointer;
     right: 15px;
     top:90px;
     font-size: 12px;
     border-radius: 7px;
     width: 60px;
     height: 60px;
     background-color: white;
     padding-top: 7px;
      i{
        font-size: 22px;
        color: #65BC7B;
      }
      span{
        font-size: 12px;
      }
   }
}

.jumbo-left{
  height: 300px;
  color: white;
   .fc-btn-our-services{
     border: none;
     margin-top: 20px;
     border-radius: 15px;
     background-color: white;
     color: black;
     padding: 15px;
     width: 200px;
     font-size: 20px;
     border: 2px solid white;
     transition: all 0.3s;
      i{
        margin-left: 5px;
      }
   }
   .fc-btn-our-services:hover{
     color: white;
     background-color: transparent;
   }
   h1{
     font-size: 70px;
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
  padding-left: 70px;
}

.contact-card{
  height: 640px;
  width: 460px;
  border-radius: 10px;
  text-align: center;
  padding: 15px;
  background-color:white;
  box-shadow: 10px 10px 30px;
   .fa-phone-alt{
          color: $primary-color;
          padding-bottom: 25px;
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
      font-size: 20px;
      padding: 12px;
    }
   input{
     width: 90%;
     padding: 20px;
     border: 1px solid lightgrey;
     border-radius: 10px;
     margin: 10px;
     outline: none;
   }
   .fc-callback{
     width: 90%;
     margin-top: 40px;
     padding: 10px;
     border: none;
     border-radius: 10px;
     background-color: $primary-color;
     color: white;
   }
   .img-card-top{
     height: 80px;
     width: 100%;
     margin-bottom: 10px;
      img{
        height: 100%;
        border-radius: 50%;
      }
   }
}

</style>