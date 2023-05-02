<script>
import TvSeries from './partials/series.vue'
import comics from '../data/dc-comics.json'

  export default {
    name: 'Main',
    data(){
      return{
        comics
      }
    },
    components:{
      TvSeries
    }
  }
</script>

<template>
  <main>
    <div class="jumbotron"></div>
    <div class="container">
      <div class="series">
        <h1>CURRENT SERIES</h1>
        <div class="wrapper">
          <TvSeries 
          v-for="(comic, index) in comics"
          :key="index"
          :image="comic.thumb"
          :serieTitle="comic.series"
          />
        </div>
        <div class="container button"><button>LOAD MORE</button></div>
        
      </div>
    </div>
  </main>
  

</template>

<style lang="scss" scoped>
@use '../scss/general/generals' as *;
@use '../scss/general/variables' as *;

main{
  background-color: $main-bg;
}
h1{
  position: absolute;
  font-size: 25px;
  color: $footer-title;
  background-color: $navbar-hover;
  padding: 15px 25px 15px 25px;
  top: 465px;
  left: 240px;
}

.jumbotron{
  height: 400px;
  background-image: url('/img/jumbotron.jpg');
}

.wrapper{
  height: 670px;
  display: flex;
  flex-wrap: wrap;
  padding-top: 55px;
}

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
.button{
  display: flex;
  justify-content: center;
}
button{
  background-color: $navbar-hover;
  color: $footer-title;
  padding: 10px 60px 10px 60px;
  border: 1px solid $navbar-hover;
  margin-bottom: 20px;
}


</style>