<template>
  <div class="container-fluid">
      <div class="container">
          <div class="contJoin" v-for="(el,i) in JoinCo" :key="i">
              <h1>{{el.title}}</h1>
              <p>{{el.comment}}</p>
              <button>sign up ></button>
          </div>
      </div>
  </div>
</template>

<script>
export default {
 name:"MyComunities",
   data(){
        return {
            JoinCo: [

                {
                title: "Hey,Joind tu our Community",
                comment: "Nulla molestie tortor nec lectus venenatis, sed blandit dui finibusdolor at,bibendum purus"
                },
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
.container-fluid{
    min-height: 300px;
    padding:10px;
    background: url('../assets/img/join_now_cta_bg.jpg');
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    display: flex;
    flex-direction: column;
    justify-content: center;


    .container{
        display: flex;
        flex-direction: column;
        justify-content: center;

        .contJoin{
            display: flex;
            align-items: center;
            flex-direction: column;
            flex-wrap: nowrap;
            gap: 20px;
            text-align: center;
            color: white;

            h1{
                width:260px;
            }

            p{
                width:400px;
            }
            button{
                padding:10px 25px;
                background-color:#37b6cf;
                color: white;
                border: none;
                text-transform: uppercase;
                font-weight:700;
            }
        }
    }
}

</style>