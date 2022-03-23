<template>
  <div>
    <figure>
      <img :src="image" alt="">
    </figure>
    <h3 class="titleCard">{{title}}</h3>
    <p class="dateCard">{{date}}</p>
    <p class="commentCard">{{comment}}</p>
  </div>
</template>

<script>
export default {
  props:{
    image:{
      type: String,
      required: true
    },
    title:{
      type: String,
      required: true
    },
    date:{
      type: String,
      required: true
    },
    comment:{
      type: String,
      required: true
    },
  }
    
}
</script>

<style lang="scss" scoped>
.titleCard{
  color: black;
  width: 100%;
  font-size: 12px;

}
.dateCard{
  font-size: 10px;
  padding: 6px 0px;
}
.commentCard{
  padding-top: 5px;
  padding-bottom: 15px;
} 
</style>
