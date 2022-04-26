<template>
  <div class="bg-header">
    <div class="container">
      <div class="row">
        <div class="col-md-4">
          <!-- Open Hours -->
          <div class="openH font-color py-2">
            <p class="m-0 fs-6">Open Hours: Mon - Sat. - 09:00-18:00</p>
          </div>
          <!-- Open Hours -->
        </div>
        <div class="col-md-8 d-flex align-items-center justify-content-end">
          <!-- Telephone number/mail/social info -->
          <div class="telephone font-color">
            <ul class="list-group d-flex flex-row">
              <li class=""><a href="#">+1(305)1234-5678</a></li>
              <li><a href="#"> hello@example.com</a></li>
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
