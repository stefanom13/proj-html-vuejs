<template>
  <div class="container-fluid">
      <div class="container">
          <div class="rowInfo">
            <h1>Tech Forum !</h1>
            <p>Discuss all the latest technologies news and trends</p>
            <button>Get Avada now! > </button>
          </div>
      </div>
      <section class="infoGeneral">
        <div class="containerInfoGeneral">
          <div class="row">
           <h2>avada   forum   is  the  place  to  be</h2>
           <p>
            In quis lectus sed leo elementum faucibus in dapibus dictum.
            Nulla molestie tortor nec lectus venenatis, sed blandit dui finibus.
            dolor at,bibendum purus.Donec vehicula nec tortor ac finibus.
          </p>
          </div>
        </div>
      </section>
  </div>
</template>

<script>

export default {
  name: 'MyMain',
  components: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container-fluid{
    min-height:500px;
    background: url('../assets/img/home_slider_bg.jpg');
    background-repeat: no-repeat;
    // background-position: center;
    background-size: cover;

    .container{
        display:flex;
        height:500px;
        flex-direction: column;
        justify-content: center;
        
        
        .rowInfo{        
            display: flex;
            flex-direction: column;
            gap: 25px;
            

            button{
              width: 180px;
              text-align: center;
              padding: 10px 15px;
              color: white;
              background-color:#27aabe;
              border: none;
              text-transform: uppercase;
              font-weight:700;
              font-size: 12px;
              cursor: pointer;
            }
            h1{
              font-size: 64px;
              color: white;
              width: 500px;
            }
            p{
              color:#aeaeae;
              font-size: 14px;
            }
        }
    }
    .infoGeneral{
      height:250px;
      background-color:#eee3d6;
      display:flex;
      align-items: center;
      justify-content: center;

      .containerInfoGeneral{
        max-width: 1000px;
        margin: 0 auto;
        text-align: center;
       

        .row{
          width: 470px;
          height: 150px;
          display:flex;
          flex-direction: column;
          align-items: center;
          justify-content: center;
          gap: 10px;

          h2{
            text-transform: uppercase;
            font-size: 12px;
            font-weight: 700;
          }

          p{
            color:#8d8d8d;
            line-height: 28px;
          }
        }

      }
    }
}
</style>
