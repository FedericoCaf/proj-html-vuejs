<template>
 <div class="wrapper">
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

  <div class="container-gray bg-light">
    <div class="container">
      <div class="marketing-title d-flex justify-content-between">
         <h2>Marketing Resources: Insider Advice on How to Increase Online Sales</h2>
         <button class="fc-button-orange">Explore All Resources</button>
      </div>
       
       <div class="row img-blog-section">

         <div v-for="(article, index) in articles" :key="index" class="col-4">
           <div class="marketing-img">
             <img :src="article.img" :alt="article.title">
           </div>
           <h3> {{article.title}} </h3>
         </div>

       </div>


    </div>
  </div>

 </div>


  
</template>

<script>
export default {
 name: 'Marketing',

   data(){
   return{
     articles:[
       {
         img: require("../assets/img/blog-posts-6-400x267.jpg"),
         title: 'Marketing Tips And Tricks For Your Website',
       },
       {
         img: require("../assets/img/blog-posts-5-400x267.jpg"),
         title: 'How to Write Stunning Blog Post Titles',
       },
       {
         img: require("../assets/img/blog-posts-4-400x267.jpg"),
         title: 'Techniques to Reduce Facebook Ads Spend',
       },
   
     ]
   }
 }

}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';

.img-testimonial{
  padding: 60px 0;
   img{
     border-radius: 10px;
   }
}

.text-testimonial{
  padding: 150px;
   h2{
     margin-bottom: 35px;
   }
}

.marketing-title{
   h2{
     width: 50%;
     font-size: 55px;
   }

   .fc-button-orange{
     width: 250px;
     height: 50px;
     margin-top: 140px;
   }
}

.img-blog-section{
  margin-top: 100px;
   .marketing-img{
     margin-bottom: 20px;
   }
}

.container-gray{
  padding: 150px 0;
}

</style>