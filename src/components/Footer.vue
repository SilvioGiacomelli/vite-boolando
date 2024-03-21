<script>
export default {}
</script>

<template>
<footer>
  <div class="intro-foot">
    <div class="l-footer">
      <p>Boolando s.r.l</p>
      <div>
        <ul>
          <li>Informazioni legali</li>
          <li>Informativa sulla privacy</li>
          <li>Diritto di recesso</li>
        </ul>
      </div>
    </div>
    <div class="r-footer">
      <p>Trovaci anche su</p>
      <div>
        <ul>
          <li><a href="#"><i class="fa-brands fa-x-twitter"></i></a></li>
          <li><a href="#"><i class="fa-brands fa-square-facebook"></i></a></li>
          <li><a href="#"><i class="fa-brands fa-square-instagram"></i></a></li>
          <li><a href="#"><i class="fa-brands fa-square-pinterest"></i></a></li>
          <li><a href="#"><i class="fa-brands fa-square-youtube"></i></a></li>
        </ul>
      </div>
    </div>
</div>
</footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
@use '../assets/scss/main.scss' as *;

.intro-foot{
  max-width: 1200px;
  margin: 0 auto;
  display:flex;
  justify-content: space-between;
  align-items: center;
  height: 100%;
}
p, li{
  color: white;
  list-style: none;
} 

ul{
  display: flex;
  padding: 10px 10px 0 0;
}

i{
  padding-right: 10px;
}

footer{
  background-color: $bg-black;
}
</style>