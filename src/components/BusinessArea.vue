<template>
  <div class="bg-black text-light">
    <div class="container py-5">
      <!-- BusinessArea top text -->
      <div class="row">
        <div class="col-12">
          <div class="text">
            <p>OUR BUSINESS AREA</p>
            <h1>
              <strong>Excellence in <span>Services</span></strong>
            </h1>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-8">
          <p>
            We are leaders in providing consultancy services with a set of
            cutting-edge technologies and a team of experienced and renowned
            professionals.Thes are some option that you can hire.
          </p>
        </div>
        <!-- button -->
        <div class="col-4">
          <button class="btn btn-danger">SEE ALL</button>
        </div>
        <!-- /button -->
      </div>
      <!-- /BusinessArea top text -->
      <!-- Grid BusinessArea -->
      <div class="row g-4">
        <div class="col-4" v-for="(item, i) in title" :key="i">
          <div class="p-4 bg-dark rounded">
            <div class="icon d-flex justify-content-between">
              <!-- icona trovata ma non è uguale, devo cercarne un'altra, intanto mi salvo il nome -->
              <i class="bi bi-diagram-2 w-100"></i>
              <a href="#"> <i class="bi bi-arrow-right"></i></a>
            </div>

            <div class="text">
              <h1 class="fs-4">{{ item.argument }}</h1>
              <p>{{ item.lorem }}</p>
            </div>
          </div>
        </div>

        <!-- <div class="col-4">
          <div class="p-3 bg-dark rounded">Custom column padding</div>
        </div>
        <div class="col-4">
          <div class="p-3 border bg-dark rounded">Custom column padding</div>
        </div>
        <div class="col-4">
          <div class="p-3 border bg-dark rounded">Custom column padding</div>
        </div>
        <div class="col-4">
          <div class="p-3 border bg-dark">Custom column padding</div>
        </div>
        <div class="col-4">
          <div class="p-3 border bg-dark">Custom column padding</div>
        </div> -->
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
          argument: "Audit & Assurance",
          lorem: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        {
          argument: "Financial Advisory",
          lorem: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        {
          argument: "Analytics and M&A",
          lorem: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        {
          argument: "Middle Marketing",
          lorem: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        {
          argument: "Legal Consulting",
          lorem: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        {
          argument: "Regular Risk",
          lorem: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
