<script>
  export default {      
  }
</script>
<template>
  <div class="card">
    <div class="box">
      <img src="../../assets/img/1.webp" alt="">
      <div class="cuore"><h4>cuore</h4></div>
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
}
.sconto {
  position: absolute;
  bottom: 20px;
  left: 5px
}
.cuore{
  position: absolute;
  top: 10px;
  right: 0;
}
</style>