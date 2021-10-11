<template>
  <div class="container">
    <left-drawer />
    <main-section />
  </div>
</template>

<script>
import LeftDrawer from "./LeftDrawer.vue";
import MainSection from "./MainSection.vue";
export default {
  components: { LeftDrawer, MainSection },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
  width: 100%;
  height: 100%;
  display: flex;
}
</style>
