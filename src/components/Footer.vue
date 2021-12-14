<template>

<footer>
  <div class="container-jumbo">
      <div class="container">
        <div class="row inner-container d-flex align-items-center">
            <div class="jumbo-left col-6">
              <h1>Let’s Make Things Happen</h1>
              <h4>Curabitur ac leo nunc. Vestibulum et mauris vel ante finibus maximus nec ut leo. Integer consectetur.</h4>    

              <div class="fc-line"></div>   
              <h5> “The team at Avada Marketing Consultant is fabulous. They helped us unlock our potential online and offline. We have experienced year on year growth due to their progressive approach.”</h5>
              <h4>George Anderson</h4>
              <p>Digitalbox CEO</p>

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
   <div class="container bottom-footer">
     <div class="row">
       <div class="col-5 container-footer-left d-flex flex-column justify-content-between">
         <div class="footer-left-top">
            <h2>Grow Your Online Business Strategically, and Improve Customer Retention.</h2>
            <div class="fc-social d-flex">
              <i class="fab fa-facebook-f"></i>
              <i class="fab fa-twitter"></i>
              <i class="fab fa-instagram"></i>
              <i class="fab fa-youtube"></i>
              <i class="fab fa-linkedin"></i>
              <i class="fab fa-tiktok"></i>
            </div>
         </div>
         
          <p>© 2021 • Avada Consultant • Powered by WordPress</p> 

       </div>

       <div class="col-7">
         <div class="row">
           <div class="col-3 container-footer-right d-flex flex-column justify-content-between">
             <ul>
               <li> <strong>Services</strong></li>
               <li>Marketing Plan</li>
               <li>Sales development</li>
               <li>Digital Marketing</li>
               <li>Pricing</li>
               <li>Wht Us</li>
               <li>Cases Studies</li>
             </ul>
             <p>Call Us (555) 802-1234</p>
           </div>
           <div class="col-3 container-footer-right d-flex flex-column justify-content-between">
             <ul>
              <li> <strong>Resources</strong></li>
               <li>Learning Center</li>
               <li>Video Tutorial</li>
               <li>Customers</li>
               <li>Blog</li>
             </ul>
             <p></p>
           </div>
           <div class="col-3 container-footer-right d-flex flex-column justify-content-between">
             <ul>
                <li> <strong>Company</strong></li>
               <li>Who We Are</li>
               <li>Contact Us</li>
               <li>Careers</li>
             </ul>
             <p>info@yourcompany.com</p>
           </div>
         </div>
       </div>
     </div>
   </div>
 

 </footer>
</template>

<script>
export default {
 name: 'Footer'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';


.container-jumbo{
  padding: 70px;
  background-color: black;
 
}

.jumbo-left{
  padding-right: 50px;
  color: white;
   .fc-btn-our-services{
     border: none;
     margin-top: 20px;
     border-radius: 15px;
     background-color: white;
     color: black;
     padding: 15px;
     width: 300px;
     font-size: 25px;
      i{
        margin-left: 5px;
      }
   }
   h1{
     font-size: 65px;
     font-weight: 700;
     color: white;
   }
   h4{
     font-size: 28px;
     margin: 30px 0;
   }

   .fc-line{
     margin-top: 50px;
     margin-bottom: 50px;
     height: 1px;
     background-color:gray;
     width: 100px;
   }
}

.jumbo-right{
  padding-left: 70px;
}

.contact-card{
  height: 520px;
  width: 420px;
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
     padding: 10px;
     border: 1px solid lightgrey;
     border-radius: 10px;
     margin: 10px;
     outline: none;
   }
   .fc-callback{
     width: 90%;
     margin-top: 10px;
     padding: 10px;
     border: none;
     border-radius: 10px;
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

.container-footer-left{
  height: 470px;
}

.container-footer-right{
  height: 470px;
   ul{
     padding-left: 0 !important;
   }
    li:not(:first-child){
      padding-top: 20px;
      cursor: pointer;
    }
}

.bottom-footer{
  margin-top: 100px;
   p{
     padding-bottom: 20px;
     font-size: 14px;
   }
}

.fc-social{
  i{
    padding: 30px 30px 30px 0;
    font-size: 20px;
  }
}


</style>