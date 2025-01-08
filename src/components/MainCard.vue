<script >


export default{
    data() {
      return {

       
        
      }
    },
    props:{

  cardArray:{
  type: Object,
  required:true
}

}
   

  }


</script>

<template>

<article>
    <img :src="cardArray.thumb" alt="">
    <p>{{ cardArray.series }}</p>
</article>

   
</template>

<style lang="scss" scoped>

article{
    width: calc((100% / 6) - 2rem);
    height:300px;
    margin-right: 2rem;
    margin-bottom: 3rem;
    
    
    img{
        width: 100%;
        height: 200px;
        object-fit:cover
    }

    p{
      color: white;
      text-align: center;
      margin-top: .7rem;
    }
}

</style>