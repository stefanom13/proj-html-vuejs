<template>
  <div class="hello">
    <div class="container-fluid">
      <div class="container">
        <!-- navbar -->
        <div class="row d-row">
          <figure>
            <img src="../assets/img/logo.png" alt="">
          </figure>
          <!--container list  -->
          <div class="container-list">

            <ul class="list-ul">
              <li v-for="(link,i) in links" :key="i">
                <a href="#">{{link.text}}</a>
              </li>
            </ul>
            <button class="btn">Join us</button>
            <p>icona</p>
          </div>
        </div>

      </div>
    </div>
  
  </div>
</template>

<script>
export default {
  name: 'MyHeader',
    data(){
    return {
      links: [
        {
          text: "Home",
          href: "#"
        },
        {
          text: "Apple",
          href: "#"
        },
        {
          text: "Microsoft",
          href: "#"
        },
        {
          text: "Android",
          href: "#"
        },
        {
          text: "Forum",
          href: "#"
        },
        {
          text: "Contact us",
          href: "#"
        },
        
      ]
    }
  }  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container-fluid{
  background-color: #27aabe;
  min-height:60px;
  display:flex;
  align-items: center;
 
}

.container{
  width: 1000px;

  .d-row{
    display:flex;
    align-items: center;
    justify-content: space-between;
   

    figure{
      // padding:10px;

      img{
        width:150px;
        
      }
    }
    .container-list{
      display:flex;
      align-items: center;
      gap: 30px;

      .btn{
        background-color: black;
        padding: 10px 12px;
        font-weight:700;
        color:white;
        font-size: 10px;
        border:none;
        cursor: pointer;
        text-transform: uppercase;
       
      }
    }
    .list-ul{
     display:flex;
     gap: 25px;

     li {
       a{
         font-size: 12px;
       }
     }
    }
   
  }

  
}
</style>
