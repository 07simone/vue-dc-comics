<template>
  <div>
  <button type="button" class="btn btn-primary">Primary</button>
      <div class="MenuTop content">

          <!--  cosi passiamo le informazioni attraverso questo metodo
            creandoci un v-bind per ognuno e riprendendo gli oggetti che ci servono -->                                                          
          <NewFilm 
          v-for="(element,index) in listaFilm" 
          :key=index   
            :imageThumb="element.thumb"                         
            :imagePrice="element.price"                           
            :imageSeries="element.series"
            :imageType="element.type"
            />
      </div>

    
  </div>
  
</template>

<script>

import NewFilm from './NewFilm.vue'

export default {
name: "MenuTop",
components:{
  NewFilm
},


data:function(){
  return{
    listaFilm:[
    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
        "price": "$19.99",
        "series": "Action Comics",
        "type": "comic book"
    },

    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
        "price": "$3.99",
        "series": "American Vampire 1976",
        "type": "comic book"
  },
  {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
        "price": "$16.99",
        "series": "Aquaman",
        "type": "graphic novel"
  },
  {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
        "price": "$2.99",
        "series": "Batgirl",
        "type": "comic book"
  },
  {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
        "price": "$3.99",
        "series": "Batman",
        "type": "comic book"
  },
  {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
        "price": "$2.99",
        "series": "Batman Beyond",
        "type": "comic book"
  },
  {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
        "price": "$3.99",
        "series": "Batman/Superman",
        "type": "comic book"
  },
  {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
        "price": "$4.99",
        "series": "Batman/Superman Annual",
        "type": "comic book"
  },
  {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
        "price": "$5.99",
        "series": "Batman: The Joker War Zone",
        "type": "comic book"
  },
  {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
        "price": "$6.99",
        "series": "Batman: Three Jokers",
        "type": "comic book"
  },
  {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
        "price": "$4.99",
        "series": "Batman: White Knight Presents: Harley Quinn",
        "type": "comic book"
  },
  {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
        "price": "$16.99",
        "series": "Catwoman",
        "type": "graphic novel"
  }
    ]
  }

}


}
</script>


<style scoped lang="scss">

.main{
  height: 150px;

.MenuTop{
  display: flex;
  flex-wrap: wrap;
  background-color: black;
  /* flex-direction: column; */
}

}
/* .films{

  padding: 3rem;
  color: white;
  width: calc(15% - (6rem));
  margin: 0.5rem

} 
img{
  width: 200px;
  height: 200px;
}
h1{

    font-size: 0.8rem;
    text-align: start;
  }
.content{
  background-color: black;

}
h3{
  padding-top: 2rem;
  color: white;
} 
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

