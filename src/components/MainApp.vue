<script >

import AsideMainApp from './AsideMainApp.vue'
import MainJumbotron from './MainJumbotron.vue'
import MainCardContainer from './MainCardContainer.vue'
export default{
    data() {
      return {

       
        
      }
    },
    components:{
      AsideMainApp,
      MainJumbotron,
      MainCardContainer
    },

  }

</script>

<template>

    <main>

      <MainJumbotron/>
      <MainCardContainer />

      
      <AsideMainApp/>

      
     
    </main>

   
</template>

<style lang="scss" scoped>
main{
  background-color: #242424;
  a{
    color: white;
  }
}


</style>