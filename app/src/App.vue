<template>
  <div id="app">
    
    <logo></logo>
    

    <like></like>
    
  </div>

</template>



<script>
 

import logo from "./components/logo.vue"
import like from "./components/like.vue"

export default {

  components: {

    logo,
    like

  },
  

}


</script>


<style lang="scss">

@import '@/scss/base.scss';

a{text-decoration: none;
  color: rgb(129, 129, 129);}
  a:hover{text-decoration: none;
  color: rgb(26, 150, 74);}


</style>
