<script>
import { headerMenu } from '../data/menus';

  export default {
    name: 'Header',
    data() {
      return {
        headerMenu
      }
    }
  }
</script>

<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="/img/dc-logo.png" alt="logo dc">
      </div>
      <nav>
        <ul>
          <li 
          v-for="(link, index) in headerMenu"
          :key="index">
            <a :class="{'active' : link.isActive}" :href="link.href">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
    
  </header>
</template>

<style lang="scss" scoped>
@use '../scss/general/generals' as *;
@use '../scss/general/variables' as *;

.container{
  display: flex;
  align-items: center;
  justify-content: space-between;
  min-height: 95px;
}
img{
  max-height: 65px;
}
ul{
  display: flex;
  align-items: center;
  min-height: 95px;
}

li{
  margin: 0 15px 0 15px;
  font-size: 11px ;
  font-weight: 600;

}
li:hover{
  border-bottom: solid 3px $navbar-hover;
}

a{
  text-decoration: none;
  color: $navbar-color;
}

a:hover{
    color: $navbar-hover;
}

</style>