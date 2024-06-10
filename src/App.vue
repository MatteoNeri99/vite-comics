<script setup>
import HeaderApp from './components/HeaderApp.vue'
import MainApp from './components/MainApp.vue'
import FooterApp from './components/FooterApp.vue'

createApp({
    data() {
      return {
        
      }
    },
    components:{
      HeaderApp,
      MainApp,
      FooterApp
    }
  }).mount('#app')
</script>

<template>

  <HeaderApp/>
  <MainApp/>
  <FooterApp/>

</template>

<style lang="scss" scoped>
@use './styles/variabili'
</style>
