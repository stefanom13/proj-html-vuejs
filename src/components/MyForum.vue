<template>
  <div class="container-fluid">
        <div class="contens">
          <span>read your blog </span>
          <div class="contArrow">
              <img src="../assets/ico/arrow-12_91092.png" alt="">
          </div>
        </div>
        <div class="container">
            <div class="infoForum">
                <p class="commentForum">phasellus eget mesus</p>
                <h2 class="titleForum">Forum Section</h2>
            </div>

            <div class="row">
                <div class="col" v-for="(icon,i) in iconsFirst" :key="i">
                    <figure>
                        <img :src="icon.src" alt="">
                    </figure>
                    <p>{{icon.text}}</p>
                </div>
            </div>
            <div class="row">
                <div class="col" v-for="(icon,i) in iconsSecond" :key="i">
                    <figure>
                        <img :src="icon.src" alt="">
                    </figure>
                    <p>{{icon.text}}</p>
                </div>
            </div>
        
        </div>

        <div class="contens">
            <span>go to our forum</span>
             <div class="contArrow">
              <img src="../assets/ico/arrow-12_91092.png" alt="">
            </div>
        </div>
  </div>
</template>

<script>
export default {
name: "MyForum",
    data(){
        return {
        iconsFirst: [
            {
            text: "News and Comunity",
            src:require('../assets/ico/news_newspaper_icon_177008.png'),
            }, 
             {
            text: "Apple Forum",
            src:require('../assets/ico/mac-apple-osx-desktop-software-hardware_icon-icons.com_59289.png'),
            }, 
            {
            text: "Microsoft Forum",
            src:require('../assets/ico/4202097logomicrosoftmswindows-115591_115710.png'),
            }, 
             {
            text: "Android Forum",
            src:require('../assets/ico/Android_icon-icons.com_66772.png'),
            }, 
            
        ],
        iconsSecond: [
            {
            text: "General Discussion",
            src:require('../assets/ico/coffecup_87565.png'),
            }, 
             {
            text: "Apps & Software",
            src:require('../assets/ico/apps_120985.png'),
            }, 
            {
            text: "Gadget & Stuff",
            src:require('../assets/ico/pc-with-monitor_icon-icons.com_56248.png'),
            }, 
             {
            text: "Tutorial & Guides",
            src:require('../assets/ico/4014703-driver-mobile-phone-repair-screw-service-wrench_112878.png'),
            }, 
            
        ],
        }
  }  

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
        display:flex;
        align-items:center;
        justify-content:center;
        gap: 7px;

        span{
            color: white;
            text-transform: uppercase;
            font-size: 12px;
            font-weight:700;
        }
        .contArrow{
          width:25px;
        }
    }
    .container{
        min-height:300px;
        display:flex;
        flex-direction:column;
        align-items:center;
        padding:10px 0px;
        background-color:#eee3d6;

        .infoForum{
            text-align:center;

            .commentForum{
                padding-top:15px;
                letter-spacing: 2px;;
            }
            .titleForum{
                padding-top:15px;
                font-size: 30px;
                padding-bottom: 25px;
            }
        }

        .row{
            width:95%;
            display:flex;
            align-items:center;
            padding:10px 0px;
            gap: 40px;
            .col{
                width: calc( 100% / 4 );
                padding:10px;
                display:flex;
                align-items: center;
                flex-direction:column;
                background-color:white;
                border-top: 2px solid #27aabe;

                figure{
                   overflow: hidden;
                    border-radius: 9999px;
                    padding:15px;
                    background-color: #fc8c5e;
                }
                p{
                    padding-top:10px;
                    padding-bottom: 30px;
                    font-weight:700;
                }
            }
        }
        
    }
}
</style>