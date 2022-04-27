<template>
  <div class="jumbotron bg-black">
    <div class="container-md p-4">
      <div class="row g-4 py-5">
        <div class="col-3">
          <div class="p-4 bg-dark rounded">
            <div class="text">
              <h1 class="fs-4">lol</h1>
            </div>
          </div>
        </div>
        <div class="col-3">
          <div class="p-4 bg-dark rounded">
            <div class="text">
              <h1 class="fs-4">lol</h1>
            </div>
          </div>
        </div>
        <div class="col-3">
          <div class="p-4 bg-dark rounded">
            <div class="text">
              <h1 class="fs-4">lol</h1>
            </div>
          </div>
        </div>
        <div class="col-3">
          <div class="p-4 bg-dark rounded">
            <div class="text">
              <h1 class="fs-4">lol</h1>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "JumbotronFooter",
};
</script>

<style scoped lang="scss">
@import "@/style/mixin";

.jumbotron {
  height: 500px;
  background-image: url("../assets/img/bg-7.jpg");
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
  padding-left: 30px;
  padding-top: 15px;
  padding-bottom: 15px;
  color: $bg-btn;
  background-color: #52b9bb60;
  border-radius: 40px 0 0 40px;
}
</style>
