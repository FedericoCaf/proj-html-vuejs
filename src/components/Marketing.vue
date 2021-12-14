<template>

  <div class="container">
      <div class="row d-flex">

         <div class="col-6 img-testimonial">
           <img src="../assets/img/large-testimonial-600x583.jpg" alt="img-testimonial">
         </div>

          <div class="col-6 text-testimonial">
              <h2>“The team at Avada Marketing Consultant is fabulous. They helped us unlock our potential online and offline. We have experienced year on year growth due to their progressive approach.”</h2>
              <h5>Kate Schadler</h5>
              <p>Marketing Consultant – Abstract</p>
              
       </div>


      </div>
  </div>
  
</template>

<script>
export default {
 name: 'Marketing'
}
</script>

<style lang="scss" scoped>

.img-testimonial{
  padding: 60px 0;
   img{
     border-radius: 10px;
   }
}

.text-testimonial{
  padding: 130px;
   h2{
     margin-bottom: 35px;
   }
}

</style>