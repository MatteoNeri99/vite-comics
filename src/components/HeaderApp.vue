<script>
export default{
  data() {
      return {

        headerLinks:[
          {
            title: 'charaters',
            link:'#',
            id: 1

          },
          {
            title: 'comics',
            link:'#',
            id: 2

          },
          {
            title: 'movies',
            link:'#',
            id: 3

          },
          {
            title: 'tv',
            link:'#',
            id: 4

          },
          {
            title: 'games',
            link:'#',
            id: 5

          },
          {
            title: 'collectibles',
            link:'#',
            id: 6

          },
          {
            title: 'videos',
            link:'#',
            id: 7

          },
          {
            title: 'fans',
            link:'#',
            id: 8

          },
          {
            title: 'news',
            link:'#',
            id: 9

          },
          {
            title: 'shop',
            link:'#',
            id: 10

          }
        ]
        
      }
    }
}
   
 

</script>

<template>

  <header>

    <img src="../assets/img/dc-logo.png" alt="">

    <nav>
      <ul>

        <li  v-for="(element, index) in headerLinks" key="element.id"><a :href="element.link">{{ element.title }}</a> </li>
      
      </ul>

    </nav>

</header>
 
</template>

<style lang="scss" scoped>

header{
  display: flex;

  ul{
    display: flex;
    list-style-type: none;

    li{
      margin-right: 2rem;

      a{
        text-decoration: none;
        color: black;
        text-transform: uppercase;
      }
    }
  }
}


</style>
