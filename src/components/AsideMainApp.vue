<script >
export default{
    data() {
      return {

        asideLinks:[
            {
                img:'./src/assets/img/buy-comics-digital-comics.png',
                title: 'digital comics',
                id:1


            },
            {
                img:'./src/assets/img/buy-comics-merchandise.png',
                title: 'dc merchandise',
                id:2


            },
            {
                img:'./src/assets/img/buy-comics-subscriptions.png',
                title: 'subscription',
                id:3


            },
            {
                img:'./src/assets/img/buy-comics-shop-locator.png',
                title: 'comic shop locato',
                id:4


            },
            {
                img:'./src/assets/img/buy-dc-power-visa.svg',
                title: 'dc power visa',
                id:5


            }
        ]


        

      }
    }
  }

</script>

<template>
<aside>

    <ul>
        <li v-for="element in asideLinks" :key="element.id">
            <img :src="element.img" alt="item.text ">
            <a href="">{{ element.title }}</a>
        </li>
    </ul>

</aside>

</template>

<style lang="scss" scoped>

aside{
  background-color: #0282f9 ;
  padding: 3rem 16rem;

    ul{
        display: flex;
        justify-content: space-around;

        li{
            display: flex;
            justify-content:center;
            align-items: center;

            img{
                width: 50px;
                margin-right: 1.5rem;
            }

            a{
                text-transform: uppercase;
                color: white;
                font-weight: bolder;
            }

        }

    }

       
 
            
}




</style>