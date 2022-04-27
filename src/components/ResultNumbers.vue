<template>
  <div class="jumbotron">
    <div class="container-md p-5">
      <!-- Text Results Numbers -->
      <div class="row gy-5">
        <div class="col-12 text-white">
          <div class="text-results text-center py-4">
            <p class="font_color">WHAT ARE WE DOING</p>
            <h1>
              <strong><span>Results</span> in Numbers</strong>
            </h1>
          </div>
        </div>
      </div>
      <!-- /Text Results Numbers -->
      <div class="row p_top">
        <div class="col-12">
          <div class="row">
            <div
              class="col-sm-2 col-md-3 text-center"
              v-for="(item, i) in results"
              :key="i"
            >
              <div class="text-results text-white">
                <h5 class="font_color">
                  <strong>{{ item.number }}</strong>
                </h5>
                <p>
                  <strong>{{ item.txt }}</strong>
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ResultNumbers",
  data() {
    return {
      results: [
        {
          number: 128,
          txt: "Certification",
        },
        {
          number: 230,
          txt: "Employees",
        },
        {
          number: 517,
          txt: "Customers",
        },
        {
          number: 94,
          txt: "Countries Served",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/mixin";
.jumbotron {
  height: 400px;
  background-image: url("../assets/img/city2.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: bottom;
  // filter: grayscale(100%) brightness(0.4);
}
span {
  background-color: $bg-opacity;
  padding: 0px 10px 0px 10px;
  border-radius: 5px;
}
.font_color {
  color: $btn-dark-green;
  font-weight: 700;
}
.p_top {
  padding-top: 50px;
}
</style>
