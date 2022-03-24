<template>
  <div class="container-fluid">
      <div class="container">
          <div class="colImg">

            <div class="contPromotions">
                <p class="titleArticle">Reviewed Product</p>
                <h1>Mauris viverra atisan ipsum eget felis primis efficitur varius</h1>
                <p>in quis lectus sed leo elementum faucibus in dapibus dictum, Nullamolestie tortur nec lectus, sed blandit dui, dolor at bibendum.</p>
                <button>Read more </button>
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
          img:require('../assets/img/post_feat_img_23-147x118.jpg'),
          title: "Donec ornare pretium eget scelisque justo",
          comment: "October 11th, 2015 | Commento off"
        },
        {
          img:require('../assets/img/post_feat_img_22-147x118.jpg'),
          title: "Fusce sollicitudin nunc sed placerat varius",
          comment: "October 11th, 2015 | Commento off"
        },
        {
          img:require('../assets/img/post_feat_img_20-147x118.jpg'),
          title: "Proin eu purus sed aru aliquet curabir vens",
          comment: "October 11th, 2015 | Commento off"
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
                h1{
                    color: white;
                    padding:10px 0;
                    font-style:italic;
                }
                .titleArticle{
                    text-transform: uppercase;
                    padding:10px 0;
                    letter-spacing:2px;
                }
                p{
                    color: rgba(255, 255, 255, 0.719);
                    padding:10px 0;
                    font-size: 14px;
                    line-height:23px;
                }
                button{
                    padding:10px 25px;
                    background-color:black;
                    color: white;
                    border: none;
                }
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
                gap: 10px;
                padding-bottom: 4px;


                figure{
                
                    img{
                        background-repeat: no-repeat;
                        background-position: center;
                        background-size: cover;
                    }
                }
                .contInfo{
                    padding-top:3px;
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