<template>
  <div class="bg-container">
    <div class="container-md p_gioia">
      <div class="row">
        <div class="col-12">
          <h6 class="font_color py-2">
            <strong>OUR EDITORIAL CONTENT</strong>
          </h6>

          <h1>
            <strong>Latest <span class="bg-opacity"> News</span> </strong>
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

            <button class="btn btn_hover">SEE ALL</button>
          </div>
        </div>
      </div>
      <div class="row g-3">
        <div
          class="col-4 align-items-center"
          v-for="(item, i) in news"
          :key="i"
        >
          <div class="rounded position-relative text-white">
            <img
              :src="require(`@/assets/img/${item.image}`)"
              alt="item"
              class="w-100 rounded"
            />
            <div class="text-absolute position_absolute w-75 text-center">
              <p>{{ item.txt }}</p>
            </div>
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
      showMore: 3,
      isShow: false,
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
        {
          image: "news-4.jpg",
          txt: "Increasing creativity is possible for everyone",
        },
        {
          image: "news-5.jpg",
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

.btn_hover {
  color: black;
}
.position_absolute {
  position: absolute;
  bottom: 10%;
  left: 10%;
}
</style>
