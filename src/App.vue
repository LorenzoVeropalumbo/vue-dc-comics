<template>
  <div id="app" class="container">
    <DcHeaderComp />
  </div>
</template>


<script>
  //IMPORTS
  import DcHeaderComp from "./components/DcHeaderComp.vue";

  export default {
    name: 'App',
    components: {
      DcHeaderComp,
    }
  }
</script>

<style lang="scss">
  @import "./style/common";
</style>
