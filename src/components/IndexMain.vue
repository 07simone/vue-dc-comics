<template>
  <div class="main">

    <MainFilms/>
    <MainCard/>

    <section class="liste">
      
            <div class="contatti-1">
                <h3>
                    DC COMICS
                </h3>
                <ul>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>TV</li>
                    <li>Games</li>
                    <li>Videos</li>
                    <li>News</li>
                </ul>

                <h3></h3>

                <h3>SHOP</h3>
                <ul>
                    <li>Shop DC</li>
                    <li>Shop DC Collectibles</li>
                </ul>
            </div>

            <div class="contatti-2">
                <h3>DC</h3>
                <ul>
                    <li>Terms Of Use</li>
                    <li>Privacy policy (new)</li>
                    <li>Ad Choices</li>
                    <li>Advertising</li>
                    <li>Jobs</li>
                    <li>Subscriptions</li>
                    <li>Talent Workshop</li>
                    <li>CPSC Certificates</li>
                    <li>Ratings</li>
                    <li>Shop Help</li>
                    <li>Contact Us</li>
                </ul>
            </div>

            <div class="contatti-3">
                <h3>
                    Sites
                </h3>

                <ul>
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>Dc Kids</li>
                    <li>Dc Universe</li>
                    <li>Dc Power Visa</li>
                </ul>
            </div>
          
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



.bonus{
  background-color: rgb(0, 83, 207);
}
.liste {
        background-image: url('../assets/img/footer-bg.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        height: 480px;
        color: white;
        display: flex;
        padding-top: 1rem;
    }
ul{

        list-style-type: none;
        padding: 0;
        
& li{
  margin-bottom: .3rem;
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
