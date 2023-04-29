<script>
export default {
  name:'Footer',
  data(){
    return{

    }
  }
}
</script>

<template>
  <div id="main-wrapper">
    <!-- PRIMA SEZIONE -->
    <div id="footer-info">
      <!-- CONTENITORE LISTE -->
      <div id="lista-info-container">
        <!-- LISTE DI SINISTRA -->
        <div id="aside-sinistro">
          <div id="list-top">          
            <h4>DC COMICS</h4>
            <ul>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movie</li>
              <li>Tv</li>
              <li>Games</li>
              <li>Videos</li>
              <li>News</li>
            </ul></div>
          <div id="list-bottom">
            <h4>SHOP</h4>
            <ul>
              <li>Shop DC</li>
              <li>Shop DC Collectibles</li>
            </ul>
          </div>
        </div>
        <!-- LISTE DESTRA -->
        <div id="aside-destro">
          <!-- LISTA DI SINISTRA -->
          <div id="list-left">
            <h4>DC</h4>
            <ul>
              <li>Terms Of Use</li>
              <li>Privacy policy(New)</li>
              <li>Ad Choices</li>
              <li>Advertisings</li>
              <li>Jobs</li>
              <li>Subscriptions</li>
              <li>Talent Workshops</li>
              <li>CPSC Certificates</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contact US</li>
            </ul>
          </div>
          <!-- LISTA DESTRA -->
          <div id="list-right">
            <h4>SITES</h4>
            <ul>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </div>
        </div>
      </div>
      <!-- SVG GIGANTE -->
      <div id="svgGigante-container"><img src="../assets/img/dc-logo-bg.png" alt=""></div>
    </div>

    <!-- SECONDA SEZIONE -->
    <div id="social">
      <div id="social-wrapper">
        <!-- SIGN_UP CONTAINER -->
        <div id="sign-up-container">
          <h3>SIGN-UP NOW!</h3>
        </div>
        <!-- FOLLOW -->
        <div id="follow-icon-container">
          <div id="follow-us-container"><h3 id="follow-us">FOLLOW US</h3></div>
          <div><img class="icon" src="../assets/img/footer-facebook.png" alt=""></div>
          <div><img class="icon" src="../assets/img/footer-twitter.png" alt=""></div>
          <div><img class="icon" src="../assets/img/footer-youtube.png" alt=""></div>
          <div><img class="icon" src="../assets/img/footer-pinterest.png" alt=""></div>
          <div><img class="icon" src="../assets/img/footer-periscope.png" alt=""></div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  #main-wrapper{
    width: 100%;
    height: 100%;
    background-image: url(../assets/img/footer-bg.jpg);
    display: flex;
    flex-direction: column;
    align-items: center;
    position: relative;
    overflow-y: hidden;
    background-size: cover;
  }

  #footer-info{
    display: flex;
    width: 70%;
    overflow-y: hidden;
  }#lista-info-container{
    padding-top: 20px;
    width: 50%;
    height: 400px;
    display: flex;
  }#aside-sinistro{
    height: 100%;
    width: 35%;
  }#list-top{
    height: 70%;
  }#list-bottom{
    height: 30%;
  }

  #svgGigante-container{
    display: flex;
    width: 50%;
    height: 100%;
    justify-content: center;
    position: absolute;
    right: 0px;
    top: -35px;
  }

  #social{
    background-color:#303030 ;
    height: 100px;
    width: 100%;
    z-index: 1;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  h4{
    color: white;
    margin-bottom: 10px;
  }

  li{
    color: #797979;
    margin-bottom: 5px;
    cursor: pointer;
  }

  li:hover{
    color: white;
  }

  #aside-destro{
    display: flex;
  }

  #list-left{
    margin-right: 10px;
  }

  #sign-up-container{
    color: white;
    padding: 2px 10px 2px 10px;
    border: 2px solid #0282f9;
    max-width: 180px;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
    &:hover{
      color: #0282f9;
    }
  }


  #social-wrapper{
    width: 70%;
    display: flex;
    justify-content: space-between;
  }

  #follow-icon-container{
    display: flex;
  }

  #follow-us-container{
    display: flex;
    justify-content: center;
    align-items: center;
  }

  #follow-us{
    color: #0282f9;
    margin-right: 15px ;
  }

.icon{
  margin-right: 5px;
  margin-left: 5px;
  cursor: pointer;
}
</style>