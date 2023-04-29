<script>
import {links} from '../data/database.js';
import imgDc from '../data/imgs.json';
import immagini from '../data/imgs.json';



export default {
  name:'Main',
  data(){
    return{
      links,
      imgDc,
      immagini,
    }
  }
}
</script>

<template>
  <!-- CONTENITORE MAIN -->
  <div id="main-wrapper">
    <!-- BANNER  -->
    <div id="jumbotron"></div>
    <!-- CONTENITORE PRINCIPALE -->
    <div id="contenuto-principale" class="black-background">
      <!-- CURRENT SERIES -->
      <div id="currentSeries"> <strong>CURRENT SERIES</strong> </div> 
      <!-- CONTENITORE IMMAGINI -->
      <div id="wrapper-immagini">
        <!-- CARD -->
        <div id="card" v-for="(immagine , i) in immagini" :key="i">
          <!-- CONTENITORE IMMAGINE -->
          <div id="imgBox"><img :src="immagine.thumb" alt=""></div>
          <div id="title">{{ immagine.series }}</div>
        </div>
      </div>

    </div>
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
    width: 100%;
    display: flex;
    justify-content: center;
    position: relative;
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
    cursor: pointer;
  }.svgName{
    font-size: small;
    margin-left: 10px;
    color: white;
  }

  .normal{
    width: 40px;
  }

  #jumbotron{
    background-image: url(../assets/img/jumbotron.jpg);
    min-height: 300px;
    background-size: cover;
  }

  #currentSeries{
    background-color: #0282f9;
    width: 180px;
    height: 50px;
    padding: 2px 4px 2px 4px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    top: -25px;
    left: 210px;
    color: white;
    font-size: large;
  }

  #wrapper-immagini{
    width: 70%;
    padding-top: 50px;
    display: flex;
    flex-wrap: wrap;
  }

  #card{
    width: calc(100% / 6);
    padding: 12px;
  }#title{
    color: white;
    font-size: large;
  }

  #imgBox{
    width: 100%;
    aspect-ratio: 2/3;
    img{
      width:100%;
      height: 100%;
      object-fit: cover;
    }
  }
</style>