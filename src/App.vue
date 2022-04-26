<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <TopHeader />
    <JumbotronHeader />
    <AdvTrailer />
  </div>
</template>

<script>
import TopHeader from "./components/TopHeader.vue";
import JumbotronHeader from "./components/JumbotronHeader.vue";
import AdvTrailer from "./components/AdvTrailer.vue";

export default {
  name: "App",
  components: {
    TopHeader,
    JumbotronHeader,
    AdvTrailer,
  },
};
</script>

<style lang="scss">
@import "@/style/utilities";
@import "@/style/mixin";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
