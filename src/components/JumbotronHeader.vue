<template>
  <div class="jumbotron">
    <div class="container">
      <div class="row py-4 align-items-center justify-content-between">
        <div class="col-2 col-sm-2 m-0">
          <!-- NavBar -->
          <div id="logo">
            <h1><span>NEX</span>GEN</h1>
          </div>
          <!-- /NavBar -->
        </div>
        <div class="col-10">
          <nav class="text-white d-flex justify-content-end">
            <ul
              v-for="(nav, i) in navBar"
              :key="i"
              class="m-0 d-flex align-items-center p-2"
            >
              <li>{{ nav }}</li>
            </ul>
            <button class="btn btn-outline-success" type="submit">
              GET IN TOUCH
            </button>
          </nav>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "JumbotronHeader",
  data() {
    return {
      navBar: ["HOME", "ABOUT", "SERVICES", "TEAM", "BLOG"],
    };
  },
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
}
#logo {
  color: white;

  h1 {
    font-size: 20px;
  }
}

#logo span {
  font-size: 20px;
  padding-left: 50px;
  padding-top: 20px;
  padding-bottom: 20px;
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
.btn_bg {
  background-color: $bg-btn;
  color: white;
}
</style>
