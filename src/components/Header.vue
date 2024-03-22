<script>
import {headerMenu} from '../data/active'

export default {
  computed:{
    leftMenu() {
      return headerMenu.left
    },
    rightMenu() {
      return headerMenu.right
    },
  }
}
</script>

<template>
  <header>
    <div class="jumbo">
      <div>
        <ul>
          <li 
          v-for="(item,index) in leftMenu"
          :key="`l-${index}`">
          <a 
          :href="item.href">{{ item.text }}</a>
        </li>         
        </ul>
      </div>
      <img
      class="logo" 
      src="../assets/img/boolean-logo.png">
      <div>
        <ul>
          <li 
          v-for="(item, index) in rightMenu"
          :key="`r-${index}`">
            <a 
            href="#"
            v-html="`${item.text}`"
            ></a>
          </li>
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

.logo{
  max-width: 50%;
  max-height: 50%;
}
</style>