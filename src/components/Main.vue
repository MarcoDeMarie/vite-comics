<script>
  export default {
    name: 'Main'
  }
</script>

<template>
  <div class="main">
    MAIN
  </div>
  
</template>

<style lang="scss" scoped>
@use '../scss/general/generals' as *;
@use '../scss/general/variables' as *;

.main{
  height: 200px;
  background-color: black;
  color: white;
  font-size: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
}


</style>