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
  <div id="main-wrapper">
    <div id="contenuto-principale" class="black-background"></div>
    <div id="barra-info" class="blu-teambg"></div>
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
  }
</style>