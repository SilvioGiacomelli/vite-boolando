<script>
import Prodotto from './partials/Prodotto.vue';
import db from '../data/db.json'
export default {
  components:{
    Prodotto
  },
data() {
  return {
    db
  }
},
}
</script>

<template>
  <main>
    <div class="container">
      <Prodotto 
      v-for="item in db.products"
      :key="item.id"
      :product="item"
      />
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
@use '../assets/scss/main.scss' as *;

.container{
  max-width: 1200px;
  display: flex;
  flex-wrap: wrap;
  margin: 0 auto;
}
</style>