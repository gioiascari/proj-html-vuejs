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
          class="col-4 align-items-center overlay_g"
          v-for="(item, i) in news"
          :key="i"
        >
          <div class="rounded position-relative text-white">
            <img
              :src="require(`@/assets/img/${item.image}`)"
              alt="item"
              class="w-100 rounded"
            />
            <div class="position_absolute-top">
              <div
                class="info-persons overlay_p gap-3 justify-content-around d-flex align-items-center"
              >
                <div class="left_g gap-2 d-flex align-items-center">
                  <i class="bi bi-person"></i>
                  <p>{{ item.nameP }}</p>
                </div>
                <div class="right_g gap-2 d-flex align-items-center">
                  <b-icon icon="clock"></b-icon>
                  <p>{{ item.day }}</p>
                </div>
              </div>
            </div>
            <div class="text-absolute position_absolute w-75 text-center">
              <h3>{{ item.title }}</h3>

              <p class="overlay_p">{{ item.txt }}</p>
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
      news: [
        {
          image: "news-1.jpg",
          title: "Increasing creativity is possible for everyone.",
          txt: " Lorem ipsum dolor sit, amet consectetur adipisicing elit.",
          nameP: "Gioia Ascari",
          day: "3 Days Ago",
        },
        {
          image: "news-2.jpg",
          title: "Because market research is part of the business plan.",
          txt: " Lorem ipsum dolor sit, amet consectetur adipisicing elit.",
          nameP: "Steven Spielberg",
          day: "8 Days Ago",
        },
        {
          image: "news-3.jpg",
          title: "Working from home is now a trend.",
          txt: " Lorem ipsum dolor sit, amet consectetur adipisicing elit.",
          nameP: "Allan Poe",
          day: "10 Days Ago",
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
.overlay_g:hover img {
  filter: blur(3px) brightness(50%);
}
.overlay_g:hover .overlay_p {
  visibility: visible;
}
.position_absolute-top {
  position: absolute;
  top: 10%;
  left: 0;
  width: 100%;
}
.left_g > p,
.right_g > p {
  margin: 0 !important;
}
.overlay_p {
  visibility: hidden;
}
</style>
