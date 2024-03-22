<script>
  export default {      
    props:{
      product: Object,
    },


methods: {
  getImagePath(img){
    return new URL (`../../assets/img/${img}`, import.meta.url).href
    }
   }
  };

</script>
<template>
  <div class="card">
    <div class="box">
      <img :src="getImagePath(product.frontImage)" alt="">
      <img class="hide" :src="getImagePath(product.backImage)" alt="">
      <div class="cuore"><h4>&#9829;</h4></div>
      <div class="sconto"><h4>sconto</h4></div>
      <div class="sostenibilità"><h4>sostenibilità</h4></div>
    </div>
    <p class="marca">Marca</p>
    <p class="stile"><h2>Stile</h2></p>
    <p class="prezzo">Prezzo</p>
  </div>
</template>


<style lang="scss" scoped>
.card{
  width: calc(100%/3);
  padding: 5px;
img{
  width: 100%;
  height: 100%;
}
}
.box{
  position: relative;
}
.sostenibilità{
  position: absolute;
  bottom:20px;
  left: 50px;
  background-color: green;
  padding: 5px;
  color: white;
  margin-left: 10px;
}
.sconto {
  position: absolute;
  bottom: 20px;
  left: 0;
  background-color: red;
  padding: 5px;
  color: white;
}
.cuore{
  position: absolute;
  top: 10px;
  right: 0;
  background-color: white;
  font-size: 2rem;
  padding: 5px;
}
.hide{
  display: none;
}
</style>