<template>
  <div class="bg-container">
    <div class="container p-4">
      <div class="row">
        <div class="col-12">
          <p>OUR EDITORIAL CONTENT</p>
          <h1>
            <strong>Latest<span> News</span> </strong>
          </h1>
        </div>
        <div class="row">
          <div
            class="col-12 d-flex justify-content-between align-items-center py-4"
          >
            <div class="text-team">
              <p class="m-0">
                Every week we publish content about what is best in the business
                world.
              </p>
            </div>
            <button class="btn btn-danger">SEE ALL</button>
          </div>
        </div>
      </div>
      <div class="row g-4">
        <div
          class="col-4 align-items-center"
          v-for="(item, i) in news"
          :key="i"
        >
          <div class="p-4 rounded position-relative text-white">
            <img
              :src="require(`@/assets/img/${item.image}`)"
              alt="item"
              class="w-100 rounded"
            />
            <p class="position-absolute fixed_bottom">{{ item.txt }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TeamAreaBottom.vue",
  data() {
    return {
      news: [
        {
          image: "news-1.jpg",
          txt: "Increasing creativity is possible for everyone",
        },
        {
          image: "news-2.jpg",
          txt: "Because market research is part of the business plan",
        },
        {
          image: "news-3.jpg",
          txt: "Working from home is now a trend",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "@/style/mixin";

.bg-container {
  background-color: $bg-news;
}
.fixed_bottom {
  bottom: 50px;
  left: 90px;
  width: 50%;
  text-align: center;
}
</style>
