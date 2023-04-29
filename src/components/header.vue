<script>
import arrayMenu from '../data/array-menu.js'; 

export default {
  name: "Header",
  data(){
    return{
      arrayMenu,
      counter: 0,

    }
  }
}
</script>

<template>
  <!-- CONTENITORE HEADER -->
  <div id="header-container" >
    <!-- CONTENITORE LOGO  -->
    <div id="main-wrapper" class="centered-flex">
      <div id="contenitore-logo" class="centered-flex">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <!-- CONTENITORE MENU -->
      <div id="contenitore-nav">
        <ul>
          <li v-for="(menuLi , i) in arrayMenu" :key="i" :class="{active : counter == i} " @click="counter = i">{{ menuLi }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>

  @use '../scss/general/general.scss';
  @use '../scss/general/typography.scss';

  #header-container{
    height: 90px;
    display: flex;
    align-items: center;
  };

  #main-wrapper{
    width: 100%;
    height: 100%;
  };

  #contenitore-logo{
    width: 40%;
    height: 100%;
    img{
      width: 70px;
    }
  };

  #contenitore-nav{
    height: 100%;
    width: 60%;
    display: flex;
    align-items: center;
    ul{
      display: flex;
      li{
        margin-left:20px;
        font-size: small;
        border-bottom: solid 5px rgba(0, 0, 255, 0);
        display: flex;
        justify-content: center;
        align-items: center;
        height: 90px;
        cursor: pointer;
        &.active{
        color: #0282f9;;
        border-bottom:solid 5px #0282f9; 
        }
      }

      li:hover{
          color: #0282f9;
          border-bottom:solid 5px #0282f9; 
        }
    }
  }


</style>