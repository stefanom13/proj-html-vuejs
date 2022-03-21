<template>
  <div class="container-fluid">
      <div class="container">
          <div class="rowInfo">
            <h1>ciao</h1>
            <p>ciaoneeee</p>
            <button>Get Avada now! > </button>
          </div>
      
      </div>
  </div>
</template>

<script>
export default {
  name: 'MyMain',
  props: {
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container-fluid{
    min-height:500px;
    background: url('../assets/img/home_slider_bg.jpg');
    background-repeat: no-repeat;
    background-position: cover;
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
            width:250px;

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

        }
    }
}
</style>
