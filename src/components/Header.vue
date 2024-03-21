<script>
export default {}
</script>

<template>
  <header>
    <div class="jumbo">
      <div>
        <ul>
          <li><a href="#">Donna</a></li>
          <li><a href="#">Uomo</a></li>
          <li><a href="#">Bambini</a></li>
        </ul>
      </div>
      <img src="../assets/img/boolean-logo.png">
      <div>
        <ul>
          <li><a href="#"><i class="fa-solid fa-user"></i></a></li>
          <li><a href="#"><i class="fa-regular fa-heart"></i></a></li>
          <li><a href="#"><i class="fa-solid fa-bag-shopping"></i></a></li>
       </ul>
     </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>

@use '../assets/scss/partials/variables' as *;
@use '../assets/scss/main.scss' as *;

header{
  background-color: $bg-orange;
  height: 60px;
  color: $color-white;
}

ul{
  display: flex;
  list-style: none;
  li{
    padding: 10px;
  }
}

.jumbo{
  margin: 0 auto;
  display:flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  height: 100%;
}

</style>