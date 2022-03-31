<template>
  <div class="films content">
        <img :src='imageThumb' :alt='imageSeries'>
        <h3>{{imageSeries}}</h3> 
      
  </div>
  
  
</template>

<script>
export default {
name: "NewFilm",
props: ['imageThumb','imagePrice','imageSeries','imageType']

}
</script>


<style scoped lang="scss">


.films{

  padding: 3rem;
  color: white;
  width: calc(15% - (6rem));
  margin: 0.5rem

}
img{
  width: 200px;
  height: 200px;
}
h3{
    padding-top: 2rem;
    color: white;
    font-size: 0.8rem;
    text-align: start;
  }

 
/* .content{
  

} */

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
