<template>
  <div id="app">
    <Site></Site>
  </div>
</template>

<script>
import Site from "./components/Site.vue";

export default {
  name: "App",
  components: {
    Site
  },
};
</script>

<style>
  @import "./css/output.css";
  @import "./css/fontImport.css";
  @import "./css/extraStyles.css";
</style>
