<template>
  <div class="main">
    <section class="content">
      <h3>-->content goes here</h3>
    </section>
    <section class="bonus">
      <div class="card">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <h5>digital comics</h5>
      </div>
      
    </section>
    <section class="liste">
      
    </section>
    
  </div>
</template>

<script>
export default {
  name: 'IndexMain',
  
}
</script>


<style scoped lang="scss">
.main{
  height: 700px;
}
.content{
  background-color: black;
  height: 100px; 
}
h3{
  padding-top: 2rem;
  color: white;
}
.card img{
  padding: 0.5rem;
}
.bonus .card{
  display: flex;
}

.liste{
  height: 450px;
 /*  background-color: yellow; */

  background-image: url(../assets/img/jumbotron.jpg);
  background-repeat: no-repeat;
  background-size: cover;
}

.bonus{
  background-color: rgb(0, 83, 207);
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
