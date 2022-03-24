<template>
  <div class="container-fluid">
      <div class="container">
          <div class="row">
              <div class="col">
                  <h3>
                      Avada tech forum
                  </h3>
                  <ul>
                      <li class="firtsComment">Lorem ipsum dolor sit amet consectetur adipisicing elit. Laboriosam tempora distinctio porro ducimus magnam praesentium?</li>
                  </ul>
              </div>
              <div class="col" v-for="(el,i) in lists" :key="i">

                  <ul>
                      <h3>{{el.title}}</h3>
                      <li>
                         {{el.comment}}
                      </li>
                       <li>
                         {{el.commentOne}}
                      </li>
                       <li>
                         {{el.commentTwo}}
                      </li>
                      <li>
                         {{el.commentTre}}
                      </li>
                  </ul>

              </div>
              
          </div>
      </div>
  </div>
</template>

<script>

export default {
 name:"MyFooter",

   data(){
        return {
            lists: [
                {
                title: "Popular Topics",
                comment: " > Lorem ipsum dolor, sit amet consectetur adipisicing elit!",
                commentOne: " > Lorem ipsum dolor, sit amet consectetur adipisicing elit.!",
                commentTwo: " > Lorem ipsum dolor, sit amet consectetur adipisicing elit.!",
                commentTre: " > Lorem ipsum dolor, sit amet consectetur adipisicing elit.!",
                },
                {
                title: "Recent Topics",
                comment: " > Lorem ipsum dolor, sit amet consectetur adipisicing elit. !",
                commentOne: " > Lorem ipsum dolor, sit amet consectetur adipisicing elit.!",
                commentTwo: " > Lorem ipsum dolor, sit amet consectetur adipisicing elit.!",
                commentTre: " > Lorem ipsum dolor, sit amet consectetur adipisicing elit.!",
                },
                {
                title: "Latiest replies",
                comment: " > Lorem ipsum dolor, sit amet consectetur adipisicing elit.",
                commentOne: " > Lorem ipsum dolor, sit amet consectetur adipisicing elit.!",
                commentTwo: " > Lorem ipsum dolor, sit amet consectetur adipisicing elit.!",
                commentTre: " > Lorem ipsum dolor, sit amet consectetur adipisicing elit.!",
                },
            ]
        }

    }
}
</script>

<style lang="scss" scoped>
.container-fluid {
    display: flex;
    align-items: center;
    padding: 30px 0px;
    border-bottom: 1px solid rgb(209, 202, 202);
    .container{
        display: flex;
        align-items: center;
        .row{
            width:1000px;
            display:flex;
            flex-direction:row;
            padding: 10px 5px;
            gap: 13px;

            .col{
                width: calc( 100% / 4 );

                h3{
                    color: black;
                    padding-bottom: 10px;
                    font-weight: 700;
                    font-size: 16px;

                }

                li{
                    color:black;
                    padding:15px 0px;
                    border-bottom: 1px solid rgb(209, 202, 202);
                    font-size: 11px;
                    font-weight: 700;
                    letter-spacing:1px;
                }
                .firtsComment{
                    color: rgba(87, 76, 76, 0.719);
                    padding:10px 0px;
                    font-size: 12px;
                    font-weight: 700;
                    border: none;
                }
            }
        }
    }
}

</style>