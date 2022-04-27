<template>
  <div class="bg-first">
    <GetInTouchTop />
    <div class="container-md py-5">
      <div class="row">
        <div class="col-12">
          <p>SEND A MESSAGE</p>
        </div>
      </div>
      <div class="row">
        <div class="col-8">
          <div class="text-team">
            <h1>
              <strong> Get in <span>Touch</span> </strong>
            </h1>
            <p>We will respond to your message as soon as possible.</p>
          </div>
          <!-- Input Messaggi -->
          <div class="controls">
            <div class="row">
              <!-- Nome -->
              <div class="col-md-6">
                <div class="form-group">
                  <input
                    id="form_name"
                    type="text"
                    name="name"
                    class="form-control"
                    placeholder="Name"
                  />
                </div>
              </div>
              <!-- /Nome -->

              <!-- Email -->
              <div class="col-md-6">
                <div class="form-group">
                  <input
                    id="Email"
                    type="text"
                    name="email"
                    class="form-control"
                    placeholder="Email"
                  />
                </div>
              </div>
              <!-- /Email -->
            </div>
            <div class="row">
              <!-- Telefono -->
              <div class="col-md-6">
                <div class="form-group">
                  <input
                    id="form_phone"
                    type="phone"
                    name="phone"
                    class="form-control"
                    placeholder="Phone"
                  />
                </div>
              </div>
              <!-- /Telefono -->

              <!-- Info -->
              <div class="col-md-6">
                <div class="form-group">
                  <input
                    id="form_info"
                    type="info"
                    name="info"
                    class="form-control"
                    placeholder="More Info"
                  />
                </div>
              </div>
              <!--/ Info -->
            </div>
            <div class="row">
              <!-- Messaggio -->

              <div class="col-md-12">
                <div class="form-group">
                  <textarea
                    id="form_message"
                    name="message"
                    class="form-control"
                    placeholder="Message"
                  ></textarea>
                </div>
              </div>

              <!-- /Messaggio -->

              <!-- BTN -->
              <div class="col-md-12">
                <button class="btn btn_hover">SEND</button>
              </div>
              <!-- / BTN -->
            </div>
          </div>
        </div>

        <!-- /Input Messaggi -->
        <!-- Data Agency -->
        <div class="col-4">
          <div class="text-president">
            <h1>Example Inc.</h1>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
          </div>

          <!-- Contatti -->
          <div class="info-contact d-flex">
            <b-icon-telephone-fill></b-icon-telephone-fill>
            <p>+1(305) 1234-5678</p>
          </div>
          <div class="info-contact d-flex">
            <b-icon-envelope-fill></b-icon-envelope-fill>4
            <p>+1(305) 1234-5678</p>
          </div>
          <div class="info-contact d-flex">
            <b-icon-telephone-fill></b-icon-telephone-fill>
            <p>+1(305) 1234-5678</p>
          </div>

          <!-- /Contatti -->
          <button class="btn btn_hover1">View Map</button>
        </div>
        <!-- /Data Agency -->
      </div>
    </div>
  </div>
</template>

<script>
import GetInTouchTop from "@/components/GetInTouchTop.vue";
export default {
  name: "GetInTouch",
  components: {
    GetInTouchTop,
  },
};
</script>

<style scoped lang="scss">
@import "@/style/mixin";
.btn_hover {
  color: black;
}
</style>
