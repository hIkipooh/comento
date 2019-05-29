<template>
  <div id="app">
    <div id="filter-sort">
      <filter-btn id="filter" />
      <sort-btn id="sort" />
    </div>
    <post-modal id="post-modal" />
    <ad-modal id="ad-modal" />
  </div>
</template>

<script>
import AdModal from "./components/AdModal.vue";
import FilterBtn from "./components/FilterBtn.vue";
import PostModal from "./components/PostModal.vue";
import SortBtn from "./components/SortBtn.vue";
import axios from "axios";

export default {
  name: "app",
  components: {
    AdModal,
    FilterBtn,
    PostModal,
    SortBtn
  },
  data() {
    return {
      posts: [],
      ads: []
    };
  },
  methods: {
    getInitialUsers() {
      for (let i = 0; i < 10; i++) {
        axios.get();
      }
    }
  }
};
</script>

<style>
#app {
  align-items: center;
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
