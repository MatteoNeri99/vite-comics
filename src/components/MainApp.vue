<script >

import AsideMainApp from './AsideMainApp.vue'
export default{
    data() {
      return {
        
      }
    },
    components:{
      AsideMainApp,
    }
  }

</script>

<template>

    <main>
      <p>--> Content goes here <--</p>
    </main>

    <AsideMainApp/>
</template>

<style lang="scss" scoped>
main{
  background-color: black;
  padding: 3rem;
  color: white;
  p{
    margin-left: 10rem;
    font-size: 2rem;
    font-weight: bold;
  }
}

</style>