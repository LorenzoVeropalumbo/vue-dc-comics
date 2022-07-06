<template>
  <header>
    <nav class="d_flex_between">
      <img src='../assets/dc-logo.png' alt="">
      
      <ul>
        <li v-for="link, index in menuLinks" :key="index" :class="{'current': link.current }"><a :href="link.url" >{{ link.text }}</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "DcHeaderComp",
  data() {
    return{
      menuLinks: [
        {
          text: 'characters',
          url: '#',
          current: false
        },
        {
          text: 'comics',
          url: '#',
          current: true
        },
        {
          text: 'movies',
          url: '#',
          current: false
        },
        {
          text: 'tv',
          url: '#',
          current: false
        },
        {
          text: 'games',
          url: '#',
          current: false
        },
        {
          text: 'collectibles',
          url: '#',
          current: false
        },
        {
          text: 'videos',
          url: '#',
          current: false
        },
        {
          text: 'fans',
          url: '#',
          current: false
        },
        {
          text: 'news',
          url: '#',
          current: false
        },
        {
          text: 'shop',
          url: '#',
          current: false
        }
      ]
    }
  },
}
</script>

<style lang="scss" scoped>
  //scss import 
  @import "../style/variables";
  header{
    
    nav{
      height: 100px;

      img{
        width: 70px;
        height: 70px;
        vertical-align: middle;
      }

      ul{
        
        display: flex;
        
        li{
          padding: 0 15px;
          text-transform: uppercase;
          font-size: 13px;
          font-weight: 600;
          color: $brand_secondary_color;
          line-height: 94px;

          &.current {
            color: $brand_main_color;          
            border-bottom: 1px solid $brand_main_color;
            border-bottom-width: 6px;
          }
        }
      }
    }
    
  }
  
</style>