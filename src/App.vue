<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <MyHeader />
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";

export default {
  name: "App",
  components: {
    MyHeader,
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
