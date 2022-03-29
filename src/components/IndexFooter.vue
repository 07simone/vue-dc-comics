<template>
  <div class="footer">
    <div class="btn">
      <button>Sign-up-now</button> 
    </div>
    <div class="social">
      <h3>FOLLOW US</h3>
      <img src="../assets/img/footer-facebook.png" alt="">
      <img src="../assets/img/footer-twitter.png" alt="">
      <img src="../assets/img/footer-youtube.png" alt="">
      <img src="../assets/img/footer-pinterest.png" alt="">
      <img src="../assets/img/footer-periscope.png" alt="">
    </div>
  

  
  </div>
</template>

<script>
export default {
  name: 'IndexFooter',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.footer{
  display: flex; 
  background-color: rgba(41, 41, 61, 0.171);
  justify-content: space-between;
}
.btn{
  align-self: center;

}
.btn button{
  display: flex;
  background-color: #494744; /* colore di sfondo    */
  border: 2px solid #0011fc; /* bordo dell'elemento */
  color: #fff;               /* colore del testo    */
  font-weight: bold;         /* testo in grassetto  */
  padding: 0.3rem;                /* padding             */
  height: 30px;              /* altezza             */
  width: 100px; 
  /* border: 1px solid blue; */
}
.social{
  display: flex;
  align-items: center;
}

.social img{
padding: 0.5rem;
}

h3{
  margin-right: 1rem;
  font-size: 1rem;
  color: blue;
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
