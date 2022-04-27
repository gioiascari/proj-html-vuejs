<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <TopHeader />
    <JumbotronHeader />
    <AdvTrailer />
    <ResultNumbers />
  </div>
</template>

<script>
import TopHeader from "./components/TopHeader.vue";
import JumbotronHeader from "./components/JumbotronHeader.vue";
import AdvTrailer from "./components/AdvTrailer.vue";
import ResultNumbers from "./components/ResultNumbers.vue";

export default {
  name: "App",
  components: {
    TopHeader,
    JumbotronHeader,
    AdvTrailer,
    ResultNumbers,
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
