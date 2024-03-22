<script>
export default {      
  props:{
    product: Object,
  },
  data() {
    return {
      // Aggiunge una variabile per controllare quale immagine mostrare
      isHovering: false,
    };
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
    <div class="box" 
    @mouseenter="isHovering = true" 
    @mouseleave="isHovering = false">
      <img class="show" :src="getImagePath(product.frontImage)" v-show="!isHovering">
      <img class="hide" :src="getImagePath(product.backImage)" v-show="isHovering">
      <div class="cuore"><h4>&#9829;</h4></div>
      <div 
        v-for="sconto in product.badges"
        :key="sconto"
        :class="sconto.type">{{ sconto.value }}
      </div>
    </div>
    <p class="marca">{{ product.brand }}</p>
    <p class="stile">{{ product.name }}</p>
    <p class="prezzo">{{ product.price }}</p>
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
.tag{
  position: absolute;
  bottom:20px;
  left: 50px;
  background-color: green;
  padding: 5px;
  color: white;
  margin-left: 10px;
}
.discount {
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

</style>