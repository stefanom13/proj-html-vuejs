<template>
 <div class="container-fluid">
    <div class="container">
      <div>
       title e compani
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
     
 </div>

  
</template>

<script>

import MyCard from './MyCard.vue'

export default {
  name: 'MyPromotions',
  components: {
    MyCard,
  },
  data(){
    return {
      firstArray:[
        {
          image:"",
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
        padding: 30px 0px;
        display: flex;
        align-items: center;
        flex-direction: column;
        gap: 10px;

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