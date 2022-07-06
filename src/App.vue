<template>
  <div id="app" >
    <DcHeaderComp class="container"/>
    <main>
      <DcMainSellComp />
      <DcMainInfo />
    </main>

    <DcFooterComp />
    <DcFooterBottom />
  </div>
</template>


<script>

  //IMPORTS
  import DcHeaderComp from "./components/DcHeaderComp.vue";
  import DcMainSellComp from "./components/DcMainSellComp.vue";
  import DcMainInfo from "./components/DcMainInfo.vue";
  import DcFooterComp from "./components/DcFooterComp.vue";
  import DcFooterBottom from "./components/DcFooterBottom.vue";

  export default {
    name: 'App',
    components: {
      DcHeaderComp,
      DcMainSellComp,
      DcMainInfo,
      DcFooterComp,
      DcFooterBottom,
    }
  }
</script>


<style lang="scss">
  //IMPORTS CSS
  @import "./style/common";
</style>
