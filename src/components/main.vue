<script>
export default {
  name:'Main',
  data(){
    return{

    }
  }
}
</script>

<template>
  <!-- CONTENITORE MAIN -->
  <div id="main-wrapper">
    <!-- CONTENITORE PRINCIPALE -->
    <div id="contenuto-principale" class="black-background"></div>
    <!-- BARRA INFO -->
    <div id="barra-info" class="blu-teambg">
      <!-- CONTENITORE DELLE SVG -->
      <div id="contenitore-svg">
        <!-- BOX INFO -->
        <div class="svg-box">
          <div class="svg"><img class="normal" src="../assets/img/buy-comics-digital-comics.png" alt=""></div>
          <div class="svgName">DIGITAL COMICS</div>
        </div>

        <div class="svg-box">
          <div class="svg"><img class="normal" src="../assets/img/buy-comics-merchandise.png" alt=""></div>
          <div class="svgName">DC MERCHANDISE</div>
        </div>

        <div class="svg-box">
          <div class="svg"><img class="normal" src="../assets/img/buy-comics-subscriptions.png" alt=""></div>
          <div class="svgName">SUBSCRIPTION</div>
        </div>

        <div class="svg-box">
          <div class="svg"><img class="w30" src="../assets/img/buy-comics-shop-locator.png" alt=""></div>
          <div class="svgName">COMIC SHOP LOCATOR</div>
        </div>

        <div class="svg-box">
          <div class="svg"><img class="normal" src="../assets/img/buy-dc-power-visa.svg" alt=""></div>
          <div class="svgName">DC POWER VISA</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  @use '../scss/general/typography.scss';

  #main-wrapper{
    width: 100%;
  }

  #contenuto-principale{
    height: 90px;
    width: 100%;
  }

  #barra-info{
    height: 110px;
    width: 100%;
    display: flex;
    justify-content: center;
  }#contenitore-svg{
    width: 75%;
    display: flex;
    align-items: center;
    justify-content: space-around;
  }.svg-box{
    display: flex;
    align-items: center;
  }.svgName{
    font-size: small;
    margin-left: 10px;
    color: white;
  }

  .svg{

  }img{

  }.normal{
    width: 40px;
  }
</style>