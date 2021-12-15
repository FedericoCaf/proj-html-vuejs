<template>

  <div class="container">

    <div v-for="(item, index) in svgContent" :key="index" class="row">
      <div v-if="(index % 2 === 0)" class="col-6 svg-container">
        <img :src="(item.img)" :alt="item.topTitle">
      </div>
      <div class="col-6 text-container">
          <h5>
            <i class="fas fa-circle fc-blue"></i> 
            {{item.topTitle}}
          </h5>
          <h1> {{item.title}} </h1>
          <p> {{item.paragraph}}
          </p>
          <button class="fc-button-orange"> {{item.button}} </button>
      </div>
      <div v-if="(index % 2 !== 0)" class="col-6 svg-container">
        <img :src="(item.img)"  :alt="item.topTitle">
      </div>
    </div>

  </div>
  
</template>

<script>
export default {
  name: 'Svgsection',

   data(){
   return{
     svgContent:[
       {
         img: require('../assets/svg/img1.svg'),
         topTitle: 'Business Growth',
         title: 'Increase Brand Awarness',
         paragraph: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed auctor placerat luctus. Nullam sit amet ante sed orci convallis gravida et at massa.',
         button: 'Get a Consultation'
       },
       {
         img: require('../assets/svg/img2.svg'),
         topTitle: 'Investors In People',
         title: 'In-House Sales Training',
         paragraph: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed auctor placerat luctus. Nullam sit amet ante sed orci convallis gravida et at massa.',
         button: 'Get a Consultation'
       },
       {
         img: require('../assets/svg/img3.svg'),
         topTitle: 'Social Media Analysis',
         title: 'Harness Your Social Proof',
         paragraph: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed auctor placerat luctus. Nullam sit amet ante sed orci convallis gravida et at massa.',
         button: 'Get a Consultation'
       },
     ]
   }
 }

}

</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

.svg-container{
  height: 600px;
  margin-top: 70px;
  // background-color: lightskyblue;
   img{
     height: 100%;
   }
}

.text-container{
   padding: 100px;
   height: 600px;
   margin-top: 100px;
   h1{
     font-size: 50px;
     font-weight: 700;
   }
    p{
      font-size: 25px;
    }
  
    .fc-button-orange{
      width: 50%;
    }
    .fa-circle.fc-blue{
      color: #0064FE;
    }
    .fa-circle.fc-yellow{
      color: #F8CC23;
    }
    .fa-circle.fc-green{
      color: #3BC77B;
    }
}

</style>