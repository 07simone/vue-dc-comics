<template>
  <div class="header">
    <img src="../assets/img/dc-logo.png" alt="">
      <ul>
          <li v-for="(element,index) in ListaNav" :key=index :class="{'active' : element.active}">
            <a :href="element.url"></a>
            <h3>{{element.name}}</h3>
            <a href="#"></a> 
          </li>
          
        
      </ul>
  </div>
</template>

<script>
export default {
  name: 'IndexHeader',
  data:function(){
    return{
      ListaNav:[
        {
          name: "Characters",
          active: false,
          url:"#"
        },
        {
          name: "comics",
          active: false,
          url:"#"
        },
        {
          name: "movies",
          active: false,
          url:"#"
        },
        {
          name: "tv",
          active: false,
          url:"#"
        },
        {
          name: "games",
          active: false,
          url:"#"
        },
        {
          name: "collectibles",
          active: false,
          url:"#"
        },
        {
          name: "video",
          active: false,
          url:"#"
        },
        {
          name: "fans",
          active: false,
          url:"#"
        },
        {
          name: "news",
          active: false,
          url:"#"
        },
        {
          name: "shop",
          active: false,
          url:"#"
        },
        
      ]
      
    }
  }
    
  
}
</script>


<style scoped lang="scss">

 *{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
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
  line-height: 12vh;
  a{
      text-decoration: none;
      
      color: black;

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
