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
          <div id="list-top"></div>
          <div id="list-bottom"></div>
        </div>
        <!-- LISTE DESTRA -->
        <div id="aside-destro"></div>
      </div>
      <!-- SVG GIGANTE -->
      <div id="svgGigante-container"></div>
    </div>

    <!-- SECONDA SEZIONE -->
    <div id="social"></div>
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
    padding-top: 30px;

  }

  #footer-info{
    background-color: green;
    display: flex;
    height: 80%;
    width: 80%;
  }#lista-info-container{
    background-color: aquamarine;
    width: 50%;
    height: 400px;
  }#aside-sinistro{
    background-color: cadetblue;
    height: 100%;
    width: 35%;
  }#list-top{
    height: 70%;
    background-color: bisque;
  }#list-bottom{
    height: 30%;
    background-color: chocolate;
  }
  
  
  #svgGigante-container{
    background-color: blue;
    width: 50%;
    height: 100%;
  }

  #social{
    margin-top: 30px;
    background-color:#303030 ;
    height: 100px;
    width: 100%;
  }
</style>