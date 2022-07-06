<template>
  <div id="app" >
    <DcHeaderComp class="container"/>
    <main>
      <DcMainSellComp />
      <DcMainInfo />
    </main>

    <DcFooterComp />
  </div>
</template>


<script>

  //IMPORTS
  import DcHeaderComp from "./components/DcHeaderComp.vue";
  import DcMainSellComp from "./components/DcMainSellComp.vue";
  import DcMainInfo from "./components/DcMainInfo.vue";
  import DcFooterComp from "./components/DcFooterComp.vue";

  export default {
    name: 'App',
    components: {
      DcHeaderComp,
      DcMainSellComp,
      DcMainInfo,
      DcFooterComp,
    }
  }
</script>


<style lang="scss">
  //IMPORTS CSS
  @import "./style/common";
</style>
