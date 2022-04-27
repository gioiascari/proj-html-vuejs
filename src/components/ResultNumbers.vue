<template>
  <div class="jumbotron">
    <div class="container p-5">
      <!-- Text Results Numbers -->
      <div class="row">
        <div class="col-12 text-white">
          <div class="text-results text-center">
            <p>WHAT ARE WE DOING</p>
            <h1>
              <strong><span>Results</span> in Numbers</strong>
            </h1>
          </div>
        </div>
      </div>
      <!-- /Text Results Numbers -->
      <div class="row">
        <div class="col-12">
          <div class="row">
            <div
              class="col-3 bg-warning"
              v-for="item in results"
              :key="item.id"
            >
              {{ item.result }}
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
          id: "",
          result: "128 Certification",
        },
        {
          id: "",
          result: "230 Employees",
        },
        {
          id: "",
          result: "517 Customers",
        },
        {
          id: "",
          result: "94 Countries Served",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.jumbotron {
  height: 450px;
  background-image: url("../assets/img/city2.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: bottom;
  // filter: grayscale(100%) brightness(0.4);
}
.text-results {
}
</style>
