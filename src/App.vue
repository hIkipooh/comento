<template>
  <div id="app">
    <div id="filter-sort">
      <filter />
      <sort />
    </div>
    <post-modal id="post-modal" />
    <ad-modal id="ad-modal" />

  </div>
</template>

<script>
import AdModal from "./components/AdModal.vue";
import Filter from "./components/Filter.vue";
import PostModal from "./components/PostModal.vue";
import Sort from "./components/Sort.vue";

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
  display: flex;
  flex-direction: column;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#filter-sort {
  display: flex;
  flex-direction: row;
  flex: 1;
}
#filter {
  flex: 1;
}
#sort {
  flex: 1;
}
#post-modal {
  flex: 3;
}
#ad-modal {
  flex: 3;
}
</style>
