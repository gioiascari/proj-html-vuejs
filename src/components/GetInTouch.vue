<template>
  <div class="bg-first">
    <GetInTouchTop />
    <div class="container-md py-5">
      <div class="row">
        <div class="col-12 font_color font_weight1">
          <p>SEND A MESSAGE</p>
        </div>
      </div>
      <div class="row">
        <div class="col-8">
          <div class="text-team">
            <h1>
              <strong> Get in <span class="bg-opacity">Touch</span> </strong>
            </h1>
            <p>We will respond to your message as soon as possible.</p>
          </div>
          <!-- Input Messaggi -->
          <div class="controls">
            <div class="row my-2">
              <!-- Nome -->
              <div class="col-md-6">
                <div class="form-group">
                  <input name="name" class="form-control" placeholder="Name" />
                </div>
              </div>
              <!-- /Nome -->

              <!-- Email -->
              <div class="col-md-6">
                <div class="form-group">
                  <input
                    name="email"
                    class="form-control"
                    placeholder="Email"
                  />
                </div>
              </div>
              <!-- /Email -->
            </div>
            <div class="row my-2">
              <!-- Telefono -->
              <div class="col-md-6">
                <div class="form-group">
                  <input
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
                    value=""
                    name="info"
                    class="form-control"
                    placeholder="More Info"
                  />
                </div>
              </div>
              <!--/ Info -->
            </div>
            <div class="row my-2">
              <!-- Messaggio -->

              <div class="col-md-12">
                <div class="form-group">
                  <textarea
                    name="message"
                    class="p-3 w-100"
                    placeholder="Message"
                  ></textarea>
                </div>
              </div>

              <!-- /Messaggio -->

              <!-- BTN -->
              <div class="col-md-12 my-2">
                <button class="btn btn_hover1">SEND</button>
              </div>
              <!-- / BTN -->
            </div>
          </div>
        </div>

        <!-- /Input Messaggi -->
        <!-- Data Agency -->
        <div class="col-4">
          <div class="text-president">
            <h1><strong> Example Inc.</strong></h1>

            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
          </div>

          <!-- Contatti -->
          <div
            class="info-contact d-flex font_color align-content-start align-items-center"
          >
            <ul>
              <li
                class="p-2 font_color"
                v-for="(contact, i) in contacts"
                :key="i"
              >
                <i
                  :class="contact.icon"
                  class="font_color bg-opacity b-radius1"
                ></i>
                {{ contact.info }}
              </li>
            </ul>
          </div>
          <div class="info-contact d-flex font_color align-items-center">
            <!-- /Contatti -->
            <button class="btn btn_hover1">VIEW MAP</button>
          </div>
          <!-- /Data Agency -->
        </div>
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
  props: ["contacts"],
};
</script>

<style scoped lang="scss">
@import "@/style/mixin";
ul {
  list-style: none;
  padding: 0;
}
.btn_hover {
  color: black;
}
.info-contact {
  p {
    margin: 0;
  }
}
.p_5 {
  padding: 5px;
}
input,
textarea {
  background-color: $bg-input;
  border: none;
}
</style>
