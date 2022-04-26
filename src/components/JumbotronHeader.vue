<template>
  <div class="jumbotron">
    <div class="container">
      <div class="row">
        <div class="col-6">
          <!-- NavBar -->
          <div id="logo">
            <h1><span>NEX</span>GEN</h1>
          </div>
          <!-- /NavBar -->
        </div>
        <div class="col-6"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "JumbotronHeader",
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
  padding-top: 50px;
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
</style>
