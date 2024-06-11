<script >
export default{
    data() {
      return {

        comicsLinks:[
            {

              title:'Charaters',
              id:1

              
            },
            {

              title:'Comics',
              id:2

              
            },
            {

            title:'Movies',
            id:3


            },
            {

            title:'TV',
            id:4


            },
            {

            title:'Games',
            id:5


            },
            {

            title:'Videos',
            id:6


            },
            {

            title:'News',
            id:6


            },
          
          
        ],

        shopLinks:[
          {
            title:'shop Dc',
            id:1
          },
          {

            title:'shop Dc Collectibles',
            id:2

          }

        ],
        dcLinks:[
            {

              title:'terms Of Use',
              id:1

              
            },
            {

              title:'Privacy Policy (New)',
              id:2

              
            },
            {

            title:'Ad Choise',
            id:3


            },
            {

            title:'Advertisng',
            id:4


            },
            {

            title:'Jobs',
            id:5


            },
            {

            title:'Subscriptions',
            id:6


            },
            {

            title:'Talent Workshops',
            id:7


            },
            {

            title:'CPSC Certificates',
            id:8


            },
            {

            title:'Ratings',
            id:9


            },
            {

            title:'Shop Help',
            id:10


            },
            {

            title:'Contacs Us',
            id:11


            },

            
            
          
          
        ],

        sitesLinks:[
          {
            title:'DC',
            id:1
          },
          {
            title:'MAD Magazine',
            id:2
          },
          {
            title:'DC Kids',
            id:3
          },
          {
            title:'DC Universe',
            id:4
          },
          {
            title:'DC Power Visa',
            id:5
          },
        ]



        
      }
    }
  }

</script>

<template>

  <footer>
    <section class="footer-link">

      <div>

        <h3>Dc comics</h3>

        <ul>
          <li v-for="element in comicsLinks" :key="element.id">
            <a href="">{{ element.title }}</a>
          </li>
        </ul>

        <h3>shop</h3>

        <ul>
          <li  v-for="element in shopLinks" :key="element.id">
            <a href=""> {{ element.title }} </a>
          </li>
        </ul>

      </div>

      <div>
        <h3>Dc</h3>

        <ul>
          <li  v-for="element in dcLinks" :key="element.id">
            <a href=""> {{ element.title }} </a>
          </li>
        </ul>

      </div>
      <div>
        <h3>sites</h3>

        <ul>
          <li  v-for="element in sitesLinks" :key="element.id">
            <a href=""> {{ element.title }} </a>
          </li>
        </ul>

      </div>

    </section>

    <img src="../assets/img/dc-logo-bg.png" alt="">
  </footer>

  
  
 
</template>

<style lang="scss" scoped>

footer{
  background-image: url(../assets/img/footer-bg.jpg);
  display: flex;
  justify-content: space-around;
  color: white;
  text-transform:uppercase ;
  font-weight: bold;

  section{
    display: flex;
    padding: 3rem ;

    h3{
      margin-bottom: 1rem;
    }

    ul{
      list-style-type: none;
      margin-right: 2rem;
      margin-bottom: 2rem;

      li{
        margin-bottom: .4rem;


        a{

          color:rgb(175, 175, 175) ;
          font-size: .8rem;

        }
      }
    }
  }
}



</style>