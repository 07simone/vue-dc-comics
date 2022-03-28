<template>
  <div class="header">
    <img src="../assets/img/dc-logo.png" alt="">
      <ul>
          <li>
            <a href="#">Characters</a> 
          </li>
          <li>
            <a href="#">comics</a> 
          </li>
          <li>
            <a href="#">movies</a> 
          </li>
          <li>
            <a href="#">tv</a> 
          </li>
          <li>
            <a href="#">gamese</a> 
          </li>
          <li>
            <a href="#">collectibles</a> 
          </li>
          <li>
            <a href="#">video</a> 
          </li>
          <li>
            <a href="#">fans</a> 
          </li>
          <li>
            <a href="#">news</a> 
          </li>
          <li>
            <a href="#">shop</a> 
          </li>
        
      </ul>
  </div>
</template>

<script>
export default {
  name: 'IndexHeader',

}
</script>


<style scoped lang="scss">

 .header{
  justify-content:space-between ;
  display: flex;
  height: 100px;
  
}


li{
  list-style-type: none;
  padding: 0.5rem;
}
ul {
  align-self: center;
  display: flex;  
  justify-content: end 
  
}

a{
  text-decoration: none;
  text-transform: uppercase;
  color: black;
 
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
