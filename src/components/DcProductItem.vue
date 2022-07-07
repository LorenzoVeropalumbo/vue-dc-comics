<template>
    <div class="wrapper">
      <img :src="productDetails.thumb"/>
      <h4>{{ productDetails.series }}</h4>     
    </div>   
</template>

<script>
  export default {
    name: "DcProductItem",
    props: {
      productDetails: Object
    }
  }
</script>

<style lang="scss" scoped>
  .wrapper {  
    margin: 18px;
    width: calc((100%/6) - 36px);
    
    img{
      height: 185px;
      width: 100%;
      object-fit: cover;
      object-position: top;
      margin: 20px 0;
    }
  }
</style>