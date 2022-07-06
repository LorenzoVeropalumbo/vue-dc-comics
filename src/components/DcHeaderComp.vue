<template>
  <header>
    <nav class="d_flex_between">
      <!-- image logo -->
      <img src='../assets/dc-logo.png' alt="">  
        <!-- Nav ul -->
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
      //Li links list
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
        width: 60%;
        display: flex;
        height: 100%;
        justify-content: space-around;

        li{
          text-transform: uppercase;
          font-size: 13px;
          font-weight: 600;
          color: $brand_secondary_color;
          height: 100%;
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