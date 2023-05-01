<script>
  export default {
    name: 'Footer'
  }
</script>

<template>
  <footer>
    <div class="container">
      <div class="footer-menu">
        <div class="col">
          <ul>
            <h3>DC COMICS</h3>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
          </ul>
          <ul>
            <h3>SHOP</h3>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
          </ul>
        </div>
        <div class="col">
          <ul>
            <h3>DC</h3>
            <li>Terms of Use</li>
            <li>Privacy policy (New)</li>
            <li>Ad Choiches</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscriptions</li>
            <li>Talent Workshop</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact Us</li>
          </ul>
        </div>
        <div class="col">
          <ul>
            <h3>SITES</h3>
            <li>DC</li>
            <li>MAD Magazine</li>
            <li>DC Kids</li>
            <li>DC Universe</li>
            <li>DC Power Visa</li>
          </ul>
        </div>
        <!-- <div class="logo">
        <img src= "/img/dc-logo-bg.png" alt="">
        </div> -->
      </div>
    </div>
    <div class="bottom">
      <div class="container container-bot">
        <button>SIGN-UP NOW!</button>
        <div class="social">
          <h2>FOLLOW US</h2>
          <img src="/img/footer-facebook.png" alt="">
          <img src="/img/footer-twitter.png" alt="">
          <img src="/img/footer-youtube.png" alt="">
          <img src="/img/footer-pinterest.png" alt="">
          <img src="/img/footer-periscope.png" alt="">
        </div>
      </div>
    </div>
  </footer>
  
</template>

<style lang="scss" scoped>
@use '../scss/general/generals' as *;
@use '../scss/general/variables' as *;

footer{
  background-image: url('/img/footer-bg.jpg');
}

// .logo{
//   left: 850px;
//   position: absolute;
// }
// .logo img{
//   width: 500px;
//   height: 500px;
// }
.footer-menu{
  display: flex;
  padding-bottom: 50px;
}
.col{
  width: 150px;
}
h2{
  color: $navbar-hover;
  margin-top: 5px;
  margin-right: 20px ;
  font-size: 20px;
}

h3{
  margin-top: 35px ;
  margin-bottom: 20px;
  color: $footer-title;
}

li{
  margin-bottom: 5px;
  font-size: 13px;
  color:$footer-list;
}

.bottom{
  background-color:$footer-bg;
  height: 90px;
}
.container-bot{
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.social{
  margin-top: 25px;
  display: flex;
}
.social img{
  margin-right: 15px;
}

button{
  margin-top: 25px;
  background-color: $footer-bg;
  color: $footer-title;
  border: 2px solid $navbar-hover;
  padding: 10px 10px 10px 10px;
}

</style>
