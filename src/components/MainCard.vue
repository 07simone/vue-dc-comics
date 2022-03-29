<template>
  <div class="CardMenuBotton">
    <div class="container">
      <ul>
        <li v-for="(element, index) in ListImg" :key=index>
          <a href="#">
            <img :src="require('../assets/img/' + element.img)" alt="">
            <h5>{{element.name}}</h5>
          </a>
        </li>

      </ul>
    </div>
  </div>
</template>

<script>
export default {
name: "CardMenuBotton",
data:function(){
    return{
            ListImg:[
              {
                img:"buy-comics-digital-comics.png",
                name:"digital comics",
                url:"#"
              },
              {
                img:"buy-comics-merchandise.png",
                name:"dc-merchandise",
                url:"#"
              },
              {
                img:"buy-comics-shop-locator.png",
                name:"subscription",
                url:"#"
              },
              {
                img:"buy-comics-subscriptions.png",
                name:"comic shop locator",
                url:"#"
              },
              {
                img:"buy-dc-power-visa.svg",
                name:" dc power visa",
                url:"#"
              }
            ]
    }
}
}
</script>


<style scoped lang="scss">

.CardMenuBotton{
  background-color: rgb(27, 49, 240);
  height: 14vh;
}
.container{
  display: flex;
  justify-content: center;
}

.header{
  justify-content:space-between ;
  display: flex;
  height: 15vh;
  
}
ul {
  height:100%;
  align-self: center;
  display: flex;  
  justify-content: end 
  
}

li{
  list-style-type: none;
  padding: 0.5rem;
  text-transform: uppercase;
  font-size: 0.8rem;
  align-self: center;
  line-height: 2vh; 
  
  a{
    
  img{
    height: 70px;
    margin-right: 0.5rem;
  }
      display: flex;
      align-items: center;
      height: 100%;
      text-decoration: none;
      display: flex;
      color:white;

    }

    &:active,
    &.active{
      border-bottom: 5px solid blue;
    }
}
/* h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
} */
</style>
