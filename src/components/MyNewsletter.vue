<template>
  <div class="container-fluid">
      <div class="container">
          <h2>Subscribe to our Newsletters</h2>
          <div class="inputCont">
            <input type="text" placeholder="Insert your email">
            <button>send</button>
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.container-fluid {
    min-height: 250px;
    padding:10px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    background-color:#eee3d6;

    .container{
        display: flex;
        flex-direction: column;
        justify-content: center;
        padding:10px;
        text-align: center;
        gap: 20px;

        .inputCont{
          display: flex;
          align-items: center;
          gap: 10px;

          input{
            width:330px;
            padding:10px;
          }
          button{
            padding:10px 26px;
            background-color:black;
            color:white;
            border: none;
            text-transform: uppercase;
            font-weight: 700;
          }
        }

      
    }
}
</style>