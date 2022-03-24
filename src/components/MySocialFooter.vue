<template>
  <div class="container-fluid">
      <div class="container">
          <p>@ Copyright 2012-2020 | Awada Theme by <span>Theme Fusion </span>| All Right Reserved | powered by <span>WordPress</span> </p>
          <div class="contIco">
            <figure  v-for="(el,i) in socials" :key="i">
                <img :src="el.src" alt="">
            </figure>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "MySocialFooter",
    data(){
        return {
            socials:[
                {
                  src:require("../assets/icoSmall/facebook_icon-icons.com_59205.png")
                },
                 {
                  src:require("../assets/icoSmall/1491579542-yumminkysocialmedia22_83078.png")
                },
                 {
                  src:require("../assets/icoSmall/1491580635-yumminkysocialmedia26_83102.png")
                },
                 {
                  src:require("../assets/icoSmall/1491580651-yumminkysocialmedia28_83061.png")
                },
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
.container-fluid{
    padding:10px;
    display: flex;
    align-items: center;

    .container{
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 1000px;
        padding: 10px 5px;;
        gap: 15px;

        p{
            font-size:12px;
        }
        span{
            font-size:12px;
            font-weight: 700;
        }
        .contIco{
            display: flex;
            align-items: center;
            gap: 10px;
            padding-right:20px;
            img{
                cursor:pointer;
            }
        }
    }
}
</style>