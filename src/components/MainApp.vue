<script >

import AsideMainApp from './AsideMainApp.vue'
import MainJumbotron from './MainJumbotron.vue'
export default{
    data() {
      return {
        
      }
    },
    components:{
      AsideMainApp,
      MainJumbotron
    }
  }

</script>

<template>

    <main>

      <MainJumbotron/>
      <AsideMainApp/>
     
    </main>

   
</template>

<style lang="scss" scoped>
main{
  background-color: black;
  color: white;


  p{
    margin-left: 10rem;
    font-size: 2rem;
    font-weight: bold;
  }
}

</style>