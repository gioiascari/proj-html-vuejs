<template>
  <div class="bg-black text-white">
    <div class="container-md p-5">
      <div class="row p-5">
        <div class="col-6">
          <div class="row">
            <div class="col-12">
              <p>NEWSLETTER</p>
              <h1>
                <strong>Know<span> First</span> </strong>
              </h1>
            </div>
            <div class="row">
              <div
                class="col-12 d-flex justify-content-between align-items-center py-4"
              >
                <div class="text-team">
                  <p class="m-0">
                    Follow closely and receive content about our company and the
                    news of the current market
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- INPUT AREA -->
        <div class="col-6">
          <form>
            <div class="form-row">
              <div class="col py-3">
                <input
                  type="text"
                  class="form-control"
                  placeholder="First name"
                />
              </div>
              <div class="col">
                <input
                  type="text"
                  class="form-control"
                  placeholder="Last name"
                />
              </div>
            </div>
            <div class="btn-container py-3">
              <button type="submit" class="btn btn_bg">SUBSCRIBE</button>
            </div>
          </form>
        </div>
        <!-- /INPUT AREA -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "GetInTouchTop",
};
</script>

<style scoped lang="scss">
@import "@/style/mixin";
.btn_bg {
  background-color: $btn-dark-green;
  color: white;
}
</style>
