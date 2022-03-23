<template>
  <div class="container-fluid">
        <div class="contens">
          <span>read your blog</span>
        </div>
        <div class="container">
            <div class="infoForum">
                <p class="commentForum">phasellus eget mesus</p>
                <h2 class="titleForum">Forum section</h2>
            </div>

            <div class="row">
                <div class="col">
                    <figure>
                        icona
                    </figure>
                    <p>testo</p>
                </div>
                <div class="col">
                    ciao
                </div>
                    <div class="col">
                    ciao
                </div>
                    <div class="col">
                    ciao
                </div>
            </div>
            <div class="row">
                <div class="col">
                    <figure>
                        icona
                    </figure>
                    <p>testo</p>
                </div>
                <div class="col">
                    ciao
                </div>
                    <div class="col">
                    ciao
                </div>
                    <div class="col">
                    ciao
                </div>
            </div>
        </div>

        <div class="contens">
            <span>go to our forum</span>
        </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.container-fluid{
    background-color:#eee3d6;
    .contens{
        // border:1px solid red;
        text-align:center;
        padding:30px 0px;
        background-color:black;

        span{
            color: white;
            text-transform: uppercase;
            font-size: 12px;
            font-weight:700;
        }
    }
    .container{
        min-height:300px;
        border:1px solid yellowgreen;
        display:flex;
        flex-direction:column;
        align-items:center;
        padding:10px 0px;
        background-color:#eee3d6;

        .infoForum{
            text-align:center;

            .commentForum{
                padding-top:15px;
            }
            .titleForum{
                padding:15px 0px;
            }
        }

        .row{
            width:95%;
            display:flex;
            align-items:center;
            padding:10px 0px;
            gap: 10px;
            .col{
                width: calc( 100% / 4 );
                padding:10px;
                display:flex;
                align-items: center;
                flex-direction:column;
                height:100px;
                background-color:white;
                border: 1px solid blue;

                figure{
                    width:40px;
                    border: 1px solid pink;
                }
            }
        }
        
    }
}
</style>