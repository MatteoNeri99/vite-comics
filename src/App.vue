<script>
import HeaderApp from './components/HeaderApp.vue'
import MainApp from './components/MainApp.vue'
import FooterApp from './components/FooterApp.vue'

export default {
    data() {
      return {
        
      }
    },
    components:{
      HeaderApp,
      MainApp,
      FooterApp
    }
  }
</script>

<template>

  <body>

    <HeaderApp/>
    <MainApp/>
    <FooterApp/>

    
  </body>


  
</template>

<style lang="scss">

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
   
  font-family: "Roboto", sans-serif;
  font-style: normal;
}


a{
  text-decoration: none;
}



</style>
