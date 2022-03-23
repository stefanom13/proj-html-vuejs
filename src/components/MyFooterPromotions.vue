<template>
  <div class="container-fluid">
      <div class="container">
          <div class="colImg">

            <div class="contPromotions">
                <h3>ciao</h3>
                <h1>ciaone</h1>
                <p>commenti</p>
                <button>botton</button>
            </div>

          </div>
          <div class="colNews">
              <h2>Tutorial & Guides</h2>
              <div class="card" v-for="(card , i) in cards" :key="i">
                  <figure>
                      <img :src="card.img" alt="">
                  </figure>
                  <div class="contInfo">
                      <p class="firstInfo">{{card.title}}</p>
                      <p class="secondInfo">{{card.comment}}</p>
                  </div>
              </div>

          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "MyFooterPromotions",
    data(){
    return {
      cards: [
        {
          img:require('../assets/img/post_feat_img_23-177x142.jpg'),
          title: "titolo",
          comment: "commento"
        },
        {
          img:require('../assets/img/post_feat_img_22-147x118.jpg'),
          title: "titolo",
          comment: "commento"
        },
        {
          img:require('../assets/img/post_feat_img_20-147x118.jpg'),
          title: "titolo",
          comment: "commento"
        },
     
        
      ]
    }
  }  

}
</script>

<style lang="scss" scoped>

.container-fluid {
    padding:20px 0px;
    .container {
        padding:20px 0px;
        display: flex;
        align-items: center;
        gap:30px;

        .colImg{
            width:68%;
            height:300px;
            background: url('../assets/img/featured_article_2_bg.jpg');
            background-repeat: no-repeat;
            background-position: center;
            background-size: cover;
            display: flex;
            flex-direction: column;
            justify-content: center;
            padding-left: 40px;

            .contPromotions{
                color: white;
            }
        }
        .colNews{
            width:28%;
            display: flex;
            flex-direction: column;
            height: 300px;

            h2{
                padding-bottom: 20px;
            }

            .card{
                
                display: flex;
                padding: 4px 0px;
                gap: 10px;


                figure{
                    width:90px;
                    
                    img{
                        background-repeat: no-repeat;
                        background-position: center;
                        background-size: cover;
                    }
                }
                .contInfo{
                    .firstInfo{
                        font-size: 13px;
                        font-weight:700;
                        padding-bottom: 10px;
                    }
                    .secondInfo{
                        font-size: 10px;
                        color:rgba(31, 11, 11, 0.719),
                    }
                }
            }
            
        }
    }
}
</style>