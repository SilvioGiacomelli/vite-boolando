<script>
import Prodotto from './partials/Prodotto.vue';
export default {
  components:{
    Prodotto
  }
}
</script>

<template>
  <main>
    <div class="container">
      <Prodotto />
      <Prodotto />
      <Prodotto />
      <Prodotto />
      <Prodotto />
      <Prodotto />
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