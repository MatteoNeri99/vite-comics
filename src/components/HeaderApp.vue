<script>
export default{
  data() {
      return {

        headerLinks:[
          {
            title: 'charaters',
            link:'#',
            active: 'false',
            id: 1

          },
          {
            title: 'comics',
            link:'#',
            active: 'true',
            id: 2

          },
          {
            title: 'movies',
            link:'#',
            active: 'false',
            id: 3

          },
          {
            title: 'tv',
            link:'#',
            active: 'false',
            id: 4

          },
          {
            title: 'games',
            link:'#',
            active: 'false',
            id: 5

          },
          {
            title: 'collectibles',
            link:'#',
            active: 'false',
            id: 6

          },
          {
            title: 'videos',
            link:'#',
            active: 'false',
            id: 7

          },
          {
            title: 'fans',
            link:'#',
            active: 'false',
            id: 8

          },
          {
            title: 'news',
            link:'#',
            active: 'false',
            id: 9

          },
          {
            title: 'shop',
            link:'#',
            active: 'false',
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

        <li  v-for="(element, index) in headerLinks" key="element.id">

          <a :href="element.link" :class="(element.active === 'true') ? 'active' : '' ">{{ element.title }}</a> 

        </li>
      
      </ul>

    </nav>

</header>
 
</template>

<style lang="scss" scoped>

header{
  display: flex;
  align-items: center;
  justify-content: space-around;
  height: 150px;

  ul{
    display: flex;
    list-style-type: none;

    li{
      margin-right: 2rem;
      

      a{
        text-decoration: none;
        color: black;
        text-transform: uppercase;
        font-weight: bold;
        padding: 3rem 0;

        &.active{
          color:#0282f9 ;
          border-bottom:2px #0282f9 solid;

        }
      }
    }
  }
}


</style>
