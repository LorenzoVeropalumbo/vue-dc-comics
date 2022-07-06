<template>
  <div id="app" >
    <DcHeaderComp class="container"/>
    <main>
      <DcMainSellComp />
      <DcMainInfo />
    </main>
  </div>
</template>


<script>

  //IMPORTS
  import DcHeaderComp from "./components/DcHeaderComp.vue";
  import DcMainSellComp from "./components/DcMainSellComp.vue";
  import DcMainInfo from "./components/DcMainInfo.vue";

  export default {
    name: 'App',
    components: {
      DcHeaderComp,
      DcMainSellComp,
      DcMainInfo,
    }
  }
</script>


<style lang="scss">
  //IMPORTS CSS
  @import "./style/common";
</style>
