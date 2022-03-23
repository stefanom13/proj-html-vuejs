<template>
 <div class="container-fluid">
    <div class="container">
      <div class="titleRow">
       <p class="paragraphRow">phasellus eget mesus</p>
       <h3>All the latest new</h3>
      </div>
      <div class="containerCard">
        <!-- card vfor article in array1 :data="article" -->
        <MyCard class="card" v-for="(el,i) in firstArray" :key="i" 
        :image="el.image" 
        :title="el.title"
        :date="el.date"
        :comment="el.comment" />
      </div>
      
    </div> 
    <MySlide/>

    <!-- <div class="container">
      <div class="containerCard">
       
      </div>
    </div> -->
 </div>

  
</template>

<script>

import MyCard from './MyCard.vue'
import MySlide from './MySlide.vue'

export default {
  name: 'MyPromotions',
  components: {
    MyCard,
    MySlide,
  },
  data(){
    return {
      firstArray:[
        {
          image:"../assets/img/post_feat_img_25-320x202.jpg",
          title:"Morbi vitae dui euismod vulputate sollicitudin",
          date:"October 11th,2015 !! 2 comments",
          comment:"Donec finibus sit amet orci eget ultricies.Praesent posuere ante ut, erat fringilla,vestibulum placerat metus mattis.Aenean dictum vitae nist",
        },
       
        
      ]
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .container-fluid {
     

      .container{
        border: 1px solid blue;
        padding: 15px 0px;
        display: flex;
        align-items: center;
        flex-direction: column;
        gap: 10px;
        .titleRow{
          text-align: center;

          .paragraphRow{
            padding:10px 0px;
            color: #727274e0;
            text-transform: uppercase;
            font-size: 12px;
            font-weight: 700;
          }
          h3{
            font-size: 30px;
            padding-bottom: 30px;
          }
        }
        .containerCard{
          display: flex;
          align-items: center;
          gap: 12px;
          // width: 100%;  
        

          .card{
            width: calc( 100% / 3 );
            padding-left: 5px;
            border:1px solid blue;
            

            figure{
              padding:10px;

              // img{
              //    display:block;
              //   aspect-ratio:1/1;
              //   object-fit:cover;
              //   object-position: center;
              // }
            }
          
          }
        }
      }
    }
</style>