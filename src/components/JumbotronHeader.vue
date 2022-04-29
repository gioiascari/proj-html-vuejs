<template>
  <div class="jumbotron">
    <div class="container-md">
      <div class="row py-4 align-items-center justify-content-between">
        <div class="col-2 col-sm-2 m-0">
          <!-- logo -->
          <div id="logo">
            <img alt="Vue logo" src="../assets/img/nexgen-logo.svg" />
          </div>
          <!-- /logo -->
        </div>
        <div class="col-10">
          <!-- NavBar -->
          <nav class="text-white d-flex justify-content-end">
            <ul
              v-for="(navBar, i) in nav"
              :key="i"
              class="m-0 d-flex align-items-center p-2"
            >
              <li>
                <a href="#"> {{ navBar }}</a>
              </li>
            </ul>
            <i class="bi bi-person d-flex p-2"></i>
            <button class="btn btn_hover" type="submit">GET IN TOUCH</button>
          </nav>
          <!-- /NavBar -->
        </div>
      </div>
      <!-- Testo centrale -->
      <div class="row">
        <div class="col-12 text-center py_5 d-flex justify-content-center">
          <div class="central-text w-50">
            <div class="title text-white">
              <h1><strong>Financial Risk</strong></h1>
              <p class="text_color">
                The right outcomes depend on continuous rigor in
                governance,models,and process across the finance function.
              </p>
            </div>
            <div class="btn-container d-flex gap-3 justify-content-center">
              <button class="btn btn_hover" type="submit">GET IN TOUCH</button>
              <button class="btn btn_hover" type="submit">READ MORE</button>
            </div>
          </div>
        </div>
      </div>
      <!-- /Testo centrale -->
    </div>
  </div>
</template>

<script>
export default {
  name: "JumbotronHeader",
  props: ["nav"],
  // data() {
  //   return {
  //     navBar: ["HOME", "ABOUT", "SERVICES", "TEAM", "BLOG"],
  //   };
  // },
};
</script>

<style scoped lang="scss">
@import "@/style/mixin";

.jumbotron {
  height: 600px;
  background-image: url("../assets/img/bg-2.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  background-blend-mode: multiply;
  background-color: rgba(0, 0, 0, 0.3);
}
#logo {
  color: white;

  h1 {
    font-size: 20px;
    font-weight: 800;
  }
}

#logo span {
  font-size: 20px;
  padding-left: 25px;
  padding-top: 10px;
  padding-bottom: 10px;
  color: $bg-btn;
  background-color: #52b9bb60;
  border-radius: 40px 0 0 40px;
}

ul {
  list-style-type: none;
  font-size: 15px;

  a {
    text-decoration: none;
    color: white;
  }
}

// Utilities
.btn_bg {
  background-color: $btn-dark-green;
  color: white;
}
.py_5 {
  padding-top: 100px;
}
</style>
