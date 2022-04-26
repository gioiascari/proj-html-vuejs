<template>
  <div class="bg-header">
    <div class="container">
      <div class="row">
        <div class="col-md-4">
          <!-- Open Hours -->
          <div class="openH font-color py-2">
            <p class="m-0 fs-6">
              <i class="bi bi-clock-fill"></i> Open Hours: Mon - Sat. -
              09:00-18:00
            </p>
          </div>
          <!-- Open Hours -->
        </div>
        <div class="col-md-8 d-flex align-items-center justify-content-end">
          <!-- Telephone number/mail/social info -->
          <div class="telephone font-color">
            <ul class="list-group d-flex flex-row">
              <li class="p-2">
                <a href="#"
                  ><i class="bi bi-telephone-fill"></i> +1(305)1234-5678</a
                >
              </li>
              <li class="p-2">
                <a href="#"
                  ><i class="bi bi-envelope-fill"></i> hello@example.com</a
                >
              </li>
              <li class="p-2"><i class="bi bi-facebook"></i></li>
              <li class="p-2"><i class="bi bi-twitter"></i></li>
              <li class="p-2"><i class="bi bi-linkedin"></i></li>
            </ul>
          </div>
          <!-- /Telephone number/mail/social info -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyHeader",
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
