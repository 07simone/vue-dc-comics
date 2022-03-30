<template>
  <div class="main">

    <MainFilms/>
    <MainCard/>


  <!--   <section class="bonus">
      <div class="card">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <h5>digital comics</h5>
      </div>
      
    </section> -->
    <section class="liste">
      
    </section>
    
  </div>
</template>


<script>

import MainFilms from './MainFilms.vue'
import MainCard from './MainCard.vue'

export default {
  name: 'IndexMain',
  components: {
    MainFilms,
    MainCard,
    
  }
}
</script>


<style scoped lang="scss">

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
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

  background-image: url(../assets/img/footer-bg.jpg);
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
