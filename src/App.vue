<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <filter />
    <sort />
    <post-modal />
    <ad-modal />

  </div>
</template>

<script>
import AdModal from "./components/AdModal.vue";
import Filter from "./components/Filter.vue";
import PostModal from "./components/PostModal.vue";
import Sort from "./components/Sort.vue";
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";

export default {
  name: "app",
  components: {
    AdModal,
    Filter,
    PostModal,
    Sort
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
