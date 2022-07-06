<template>
  <div id="app" >
    <DcHeaderComp class="container"/>
    <main>
      <DcMainSellComp />
    </main>
  </div>
</template>


<script>
  //IMPORTS
  import DcHeaderComp from "./components/DcHeaderComp.vue";
  import DcMainSellComp from "./components/DcMainSellComp.vue";

  export default {
    name: 'App',
    components: {
      DcHeaderComp,
      DcMainSellComp,
    }
  }
</script>

<style lang="scss">
  @import "./style/common";
</style>
