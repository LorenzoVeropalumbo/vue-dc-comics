<template>
  <section>
    <div class="container">
      <span class="current-series">CURRENT SERIES</span>
      <div class="container-items">
        <DcProductItem v-for="element, index in products" :key="index" :productDetails="element"/>
      </div>    
    </div>  
    <div class="load-more">
     <span>LOAD MORE</span> 
    </div> 
  </section>
</template>

<script>
  import productsJson from '../assets/dc-comics.json';
  import DcProductItem from './DcProductItem.vue';
  
  export default {
    name:"DcMainSellComp",
    components: {
      DcProductItem
    },
    data() {
      return {
        products: productsJson
      };
    }
  } 
</script>

<style lang="scss" scoped>
  @import "../style/variables";
  section{
    position: relative;
    background-color: $background_buy_section;
    color: white;
    padding: 10px 0;

      .current-series{
        font-size: 25px;
        font-weight: 600;
        position: absolute;
        padding: 10px 35px;
        bottom: calc(100% - 25px);
        left: 15%;
        font-size: 25px;
        background-color: $background_info_section;
        font-stretch: condensed;
      }

      .container-items{
        display: flex;
        flex-wrap: wrap;
      }
      .load-more{
        
        text-align: center;
        margin: 50px 0 20px;
        span{
          background-color: $background_info_section;
          padding: 10px 55px;
          font-size: 14px;
          font-weight: bold;
        }
      }
  }
</style>