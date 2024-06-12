<script >


export default{
    data() {
      return {
        
      }
    },
  
  }

</script>

<template>
    <section class="jumotron">

        <div>
            <h2>current series</h2>
        </div>


    </section>

    
</template>

<style lang="scss" scoped>


section{
    position: relative;
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);

    div{
        height: 50px;
        padding: 2rem;
        margin-left: 10rem;
        position: absolute;
        top:356px;

        h2{
            background-color:  #0282f9;
            padding: 1rem 1.6rem;
            text-transform: uppercase;
        }
    }
}
</style>