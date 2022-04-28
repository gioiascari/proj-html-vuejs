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
      <div class="row g-2">
        <div class="col-4" v-for="(item, i) in title" :key="i">
          <div class="p-4 bg-dark rounded">
            <div class="icon d-flex justify-content-between py-3">
              <img :src="require(`../assets/img/${item.icon}`)" alt="" />
              <i class="bi bi-arrow-right"></i>
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
  props: ["icons"],
  data() {
    return {
      title: [
        {
          name: "Audit & Assurance",
          icon: "audit.svg",
          txt: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
        },
        {
          name: "Financial Advisory",
          icon: "financial.svg",
          txt: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
        },
        {
          name: "Analytics and M&A",
          icon: "analytics.svg",
          txt: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
        },
        {
          name: "Middle Marketing",
          icon: "middle.svg",
          txt: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
        },
        {
          name: "Legal Consulting",
          icon: "consulting.svg",
          txt: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
        },
        {
          name: "Regular Risk",
          icon: "risk.svg",
          txt: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/mixin";

img {
  height: 50px;
  color: $color-green;
  filter: invert(35%) sepia(80%) saturate(4880%) hue-rotate(164deg)
    brightness(89%) contrast(96%);
}
i {
  color: $color-green;
  font-size: 20px;
}
</style>
