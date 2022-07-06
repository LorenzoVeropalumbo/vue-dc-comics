<template>
  <section>
    <div class="container">
      <div v-for="info, index in menuInfo" :key="index">
        <img :src="info.img" alt="">
        <a :href="info.url">{{ info.text }}</a>
      </div>
    </div>   
  </section>
</template>

<script>
  export default {
    name:"DcMainInfo",
     data(){
      return{ 
        menuInfo: [
          {
            text: 'digital comics',
            img: require("../assets/buy-comics-digital-comics.png"),
            url: '#',     
          },
          {
            text: 'dc merchandise',
            img: require("../assets/buy-comics-merchandise.png"),
            url: '#',      
          },
          {
            text: 'subscription',
            img: require("../assets/buy-comics-subscriptions.png"),
            url: '#',     
          },
          {
            text: 'comic shop locator',
            img: require("../assets/buy-comics-shop-locator.png"),
            url: '#',   
          },
          {
            text: 'dc power visa',
            img: require("../assets/buy-dc-power-visa.svg"),
            url: '#',       
          },
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import "../style/variables";
  section{
    background-color: $background_info_section;
    color: white;
    padding: 50px 40px;

    .container{
      display: flex;
      justify-content: space-around;

      div{
        display: flex;
        align-items: center;
        
        img{
          width: 55px;
          height: 60px;
        }
        
        a{
          padding: 0 10px;
          font-size: 15px;
          font-weight: 100;
          text-transform: uppercase;
        }
      }
    }    
  }
</style>