<script>
import {links} from '../data/database.js'
export default {
  name:'Main',
  data(){
    return{
      links,
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
        <div class="svg-box" v-for="(link , i) in links" :key="i">
          <div class="svg"><img class="normal" :src="link.immagine" alt=""></div>
          <div class="svgName">{{link.nome}}</div>
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
    width: 65%;
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