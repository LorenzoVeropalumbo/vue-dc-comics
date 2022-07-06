<template>
  <section>
    <div class="container">
      <span>Content goes here</span>
    </div>   
  </section>
</template>

<script>
export default {
 name:"DcMainSellComp"
}
</script>

<style lang="scss" scoped>
  @import "../style/variables";
  section{
    background-color: $background_buy_section;
    color: white;
    padding: 50px 0;
    span{
      font-size: 25px;
      font-weight: 600;   
    }
  }
</style>