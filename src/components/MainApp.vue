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
      <div>

        <button>load more</button>

      </div>
      
      <AsideMainApp/>

      
     
    </main>

   
</template>

<style lang="scss" scoped>
main{
  background-color:#1c1c1c;;
  color: white;
  display: flex;
  flex-direction: column;

  div{
    align-self: center;

    button{
    background-color: #0282f9;
    color: white;
    border: transparent;
    padding:.7rem  5rem;
    margin-bottom: 1rem;
    text-transform: uppercase;
    font-weight: bold;
  
    }
 
  }



  p{
    margin-left: 10rem;
    font-size: 2rem;
    font-weight: bold;
  }
}

</style>