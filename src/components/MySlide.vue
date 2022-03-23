<template>
  <div class="container-fluid">
      <div class="container">
        <div class="infoSlide">
         <p class="titleArticle">featured article</p>
         <h1>Cras malesuada et orci eget pharetra</h1>
         <p class="textArticle">
            In quis lectus sed leo elementum faucibus in dapibus dictum.
            Nullamolestie tortor nec lectus veneanatis,sed blandit dui, dolor
            at bibendum sadipis ets ipsum dolores ficilis uns leo lectus
         </p>
         <button>READ MORE  > </button>
        </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .container-fluid{
        padding:5px 0px;
        .container {
            padding: 10px;
            min-height:400px;
            background: url('../assets/img/featured_article_1_bg.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            display:flex;
            flex-direction: column;
            justify-content: center;
            padding-left: 40px;

            .infoSlide{
                line-height:29px;

                .titleArticle{
                    text-transform: uppercase;
                    color: white;
                    padding:10px 0;
                }
                h1{
                    color: white;
                    padding:10px 0;
                }
                .textArticle{
                    color: rgba(255, 255, 255, 0.719);
                    padding:10px 0;
                    font-size: 14px;
                }
                button{
                    padding:10px 25px;
                    background-color:black;
                    color: white;
                    border: none;
                    
                }
            }
        }
    }
    
</style>