<script>
export default {
  name:'TvSeries',
  props:{
    image: String,
    serieTitle: String
  }

}
</script>

<template>
  <div class="card">
    <img :src="image" alt="">
    <p>{{ serieTitle }}</p>
  </div>
  
</template>

<style lang="scss" scoped>
@use '../../scss/general/generals' as *;
@use '../../scss/general/variables' as *;

.card{
  height: 200px;
  width: 200px;
  img{
    width: 100%;
    height: 100%;
    object-fit: contain;
  }
  p{
    color: $series-name;
    display: flex;
    justify-content: center;
  }
}

</style>