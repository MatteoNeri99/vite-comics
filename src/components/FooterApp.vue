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
        ],

        footerLinks:[
            {
                img:'./src/assets/img/footer-facebook.png',
                id:1


            },
            {
                img:'./src/assets/img/footer-twitter.png',
                id:2


            },
            {
                img:'./src/assets/img/footer-youtube.png',
                id:3


            },
            {
                img:'./src/assets/img/footer-pinterest.png',
                id:4


            },
            {
                img:'./src/assets/img/footer-periscope.png',
                id:5


            }
        ]



        
      }
    }
  }

</script>

<template>

  <footer>
    <div class="container">
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

    <div class="dc-logo-footer">
      
      <img src="../assets/img/dc-logo-bg.png" alt="">

    </div>

    </div>


    

    <section class="social">
      <button>sign-up now!</button>

      <div>

        <p>follow us</p>

        <div  v-for="element in footerLinks" key="element.id">

          <img :src="element.img" alt="">

        </div>
        
      </div>
    </section>


  </footer>

  
  
 
</template>

<style lang="scss" scoped>


.container{
  background-image: url(../assets/img/footer-bg.jpg);
  background-repeat: no-repeat ;
  background-size: cover;
  height: 500px;
  display: flex;
  flex-wrap: wrap;
  color: white;
  font-weight: bold;

  .dc-logo-footer{
      
      position: relative;

      img{
        position: Absolute;
        top:-50px;
        clip: Rect(50px 565px 550px 0px);
      }
    }

  section.footer-link{
    width: 50%;
    display: flex;
    height: 400px;
    padding: 3rem;
    margin-left: 10rem;
    

    h3{
      margin-bottom: 1rem;
      text-transform:uppercase ;
      
      
    }

    ul{
      list-style-type: none;
      margin-right: 2rem;
      margin-bottom: 1rem;
     
      



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
section.social{
    background-color:#303030;
    width: 100%;
    height: 100px;
    color: white;
    display: flex;
    align-items: center;
    justify-content: space-around;

    button{
      background-color: transparent;
      border: 1px solid #0282f9;
      color: white;
      text-transform: uppercase;
      padding: .5rem .7rem;
    }

    div{
      display: flex;

      img{
        margin-left: 1rem;
      }
    }
    p{
      text-transform: uppercase;
      color: #0282f9;
      font-weight: bold;
      align-self: center;
    }
  }



</style>