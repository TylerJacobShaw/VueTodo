<template>
  <div class="parent" id="app">
    <Header/>
    <router-view/>
  </div>
</template>
<script>
import Header from "./components/layout/Header";
export default {
  name: "app",
  components: {
    Header
  }
};
</script>
<style scoped>
.parent {
  max-width: 1366px;
  margin: 0 auto !important;
  float: none !important;
}
</style>
