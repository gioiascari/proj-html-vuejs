<template>
  <div class="bg-header">
    <div class="container-md">
      <div class="row">
        <div class="col-md-12 col-sm-12 d-flex justify-content-between">
          <!-- Open Hours -->
          <div class="openH py-2 text_color">
            <p class="m-0 fs-6">
              <i class="bi bi-clock-fill"></i> Open Hours: Mon - Sat. -
              09:00-18:00
            </p>
          </div>

          <!-- Open Hours -->
          <div class="telephone">
            <ul class="list-group d-flex flex-row">
              <li
                class="p-2 text_color"
                v-for="(contact, i) in contacts"
                :key="i"
              >
                <i :class="contact.icon"></i>
                {{ contact.info }}
              </li>

              <li class="p-2 text_color"><i class="bi bi-facebook"></i></li>
              <li class="p-2 text_color"><i class="bi bi-twitter"></i></li>
              <li class="p-2 text_color"><i class="bi bi-linkedin"></i></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TopHeader",
  props: ["contacts"],
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/style/mixin";
.font-color {
  color: $font-color;
}
.bg-header {
  background-color: $bg-header;
}
ul {
  list-style-type: none;
  li a {
    padding-right: 20px;
    text-decoration: none;
    color: $font-color;
  }
}
</style>
