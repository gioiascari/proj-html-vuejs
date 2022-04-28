<template>
  <div class="bg-black text-light">
    <div class="container-md py-5">
      <!-- BusinessArea top text -->
      <div class="row">
        <div class="col-12">
          <div class="text">
            <p class="font_color">OUR BUSINESS AREAS</p>
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
          <button type="button" class="btn btn_hover">SEE ALL</button>
        </div>
        <!-- /button -->
      </div>
      <!-- /BusinessArea top text -->
      <!-- Grid BusinessArea -->
      <div class="row g-2">
        <div class="col-4" v-for="(item, i) in title" :key="i">
          <div class="p-4 bg-dark rounded">
            <div class="icon d-flex justify-content-between">
              <!-- icona trovata ma non è uguale, devo cercarne un'altra, intanto mi salvo il nome -->
              <b-icon
                :icon="icon"
                v-for="(icon, j) in item.icon"
                :key="j"
              ></b-icon>
              <!-- <a href="#"> <i class="bi bi-arrow-right"></i></a> -->
            </div>

            <div class="text">
              <!-- Icone -->

              <!--/ Icone -->

              <h1 class="fs-4">{{ item.argument }}</h1>
              <p>{{ item.lorem }}</p>
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
  data() {
    return {
      title: [
        {
          icon: ["diagram2", "arrow-right"],
          argument: "Audit & Assurance",
          lorem: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        {
          icon: ["briefcase", "arrow-right"],
          argument: "Financial Advisory",
          lorem: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        {
          icon: ["bar-chart", "arrow-right"],
          argument: "Analytics and M&A",
          lorem: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        {
          icon: ["diagram2"],
          argument: "Middle Marketing",
          lorem: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        {
          icon: ["diagram2"],
          argument: "Legal Consulting",
          lorem: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        {
          icon: ["diagram2"],
          argument: "Regular Risk",
          lorem: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/mixin";

span {
  background-color: $bg-opacity;
  padding: 0px 10px 0px 10px;
  border-radius: 5px;
}
</style>
