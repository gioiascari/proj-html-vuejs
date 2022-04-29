<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <TopHeader :contacts="contacts" />
    <JumbotronHeader :nav="nav" />
    <AdvTrailer />
    <ResultNumbers />
    <BusinessArea />
    <TeamArea />
    <GetInTouch :contacts="contacts" />
    <JumbotronFooter :contacts="contacts" />
    <FooterBottom />
  </div>
</template>

<script>
import TopHeader from "./components/TopHeader.vue";
import JumbotronHeader from "./components/JumbotronHeader.vue";
import AdvTrailer from "./components/AdvTrailer.vue";
import ResultNumbers from "./components/ResultNumbers.vue";
import BusinessArea from "./components/BusinessArea.vue";
import TeamArea from "./components/TeamArea.vue";
import GetInTouch from "./components/GetInTouch.vue";
import JumbotronFooter from "./components/JumbotronFooter.vue";
import FooterBottom from "./components/FooterBottom.vue";

export default {
  name: "App",
  components: {
    TopHeader,
    JumbotronHeader,
    AdvTrailer,
    ResultNumbers,
    BusinessArea,
    TeamArea,
    GetInTouch,
    JumbotronFooter,
    FooterBottom,
  },
  data() {
    return {
      nav: ["HOME", "ABOUT", "SERVICE", "TEAM", "BLOG"],
      contacts: [
        {
          type: "phone",
          info: "+1 (305) 1234-5678",
          icon: "bi bi-telephone-fill",
        },
        {
          type: "email",
          info: "hello@example.com",
          icon: "bi bi-envelope-fill",
        },
        {
          type: "position",
          info: "Main Avenue, 987",
          icon: "bi bi-geo-alt-fill",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "@/style/utilities";
@import "@/style/mixin";

#app {
  font-family: "Poppins";
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
</style>
