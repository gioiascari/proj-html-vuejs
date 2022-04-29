<template>
  <div class="bg-black text-light">
    <div class="container-md py-5">
      <!-- BusinessArea top text -->
      <div class="row">
        <div class="col-12">
          <div class="text">
            <div class="font_color">
              <p>OUR BUSINESS AREAS</p>
            </div>

            <h1>
              <strong>Excellence in <span>Services</span></strong>
            </h1>
          </div>
        </div>
      </div>
      <div class="row justify-content-between">
        <div class="col-10">
          <p>
            We are leaders in providing consultancy services with a set of
            cutting-edge technologies and a team of experienced and renowned
            professionals.Thes are some option that you can hire.
          </p>
        </div>
        <!-- button -->
        <div class="col-2 d-flex align-items-center justify-content-end">
          <button type="button" class="btn btn_hover">SEE MORE</button>
        </div>
        <!-- /button -->
      </div>
      <!-- /BusinessArea top text -->
      <!-- Grid BusinessArea -->
      <div class="row g-4">
        <div class="col-4 overlay_g" v-for="(item, i) in title" :key="i">
          <div class="p-4 bg-dark rounded">
            <div
              class="icon py-2 d-flex justify-content-between align-items-center"
            >
              <img :src="require(`../assets/img/${item.icon}`)" alt="" />
              <div class="icon-g">
                <i class="bi bi-arrow-right p-2"></i>
              </div>
            </div>

            <div class="text">
              <h1 class="fs-4">{{ item.name }}</h1>
              <p>{{ item.txt }}</p>
            </div>
          </div>
        </div>
      </div>
      <!-- /Grid BusinessArea -->
    </div>
  </div>
</template>

<script>
export default {
  name: "BusinessArea",
  props: ["title"],
};
</script>

<style lang="scss" scoped>
@import "@/style/mixin";

img {
  height: 50px;
  filter: invert(35%) sepia(80%) saturate(4880%) hue-rotate(164deg)
    brightness(89%) contrast(96%);
}
i {
  color: $color-green;
  font-size: 20px;
}
.overlay_g:hover img {
  filter: brightness(0) invert(1);
}
.overlay_g:hover i {
  color: white;
  background-color: $color-green;
  border-radius: 50%;
}
.overlay_g:hover {
  transform: translateY(-10px);
}
.overlay_g {
  transition: transform 0.5s ease-in;
}
</style>
