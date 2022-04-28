<template>
  <div class="jumbotron bg-black">
    <div class="container-md p-4">
      <div class="row g-4 py-5 align-items-center">
        <!-- Colonna Logo e icone -->
        <div class="col-3 col-sm-6 col-md-3">
          <div class="p-4">
            <div class="logo w-75">
              <img
                alt="Vue logo"
                src="../assets/img/nexgen-logo.svg"
                class="w-100"
              />
            </div>

            <div class="text_color fs-6">
              <p>A Functional HTML Template for Corporate Business.</p>
            </div>
            <!-- Phone -->
            <div class="info-contact d-flex font_color align-items-center">
              <b-icon-telephone-fill
                style="color: #048383"
                class="text-white"
                font-scale="1"
              ></b-icon-telephone-fill>
              <div class="text-contacts p-2 text_color">
                <p>+1(305) 1234-5678</p>
              </div>
            </div>
            <!-- / PHone -->

            <!-- Mail -->
            <div class="info-contact d-flex align-items-center">
              <b-icon-envelope-fill
                style="color: #048383"
                class="text-white"
                font-scale="1"
              ></b-icon-envelope-fill>
              <div class="text-contacts p-2 text_color">
                <p>hello@example.com</p>
              </div>
            </div>
            <!-- / Mail -->

            <!-- Addres -->
            <div class="info-contact d-flex text_color align-items-center">
              <b-icon-telephone-fill
                style="color: #048383"
                class="text-white"
                font-scale="1"
              ></b-icon-telephone-fill>
              <div class="text-contacts p-2 text_color">
                <p>Main Avenue, 987</p>
              </div>
            </div>
            <!-- / Addres -->
            <button class="btn btn_hover" type="submit">GET IN TOUCH</button>
          </div>
        </div>
        <!-- /Colonna Logo e icone -->

        <!-- About col -->
        <div class="col-3 col-sm-6 col-md-3">
          <div class="p-4 bg-dark rounded">
            <div class="text-white">
              <h1 class="fs-4">About</h1>
              <ul>
                <li><a href="#"> The Company</a></li>
                <li><a href="#"> Insitutional</a></li>
                <li><a href="#"> Social Events</a></li>
                <li><a href="#"> Innovation</a></li>
                <li><a href="#"> Environment</a></li>
                <li><a href="#"> Technology</a></li>
              </ul>
            </div>
          </div>
        </div>
        <!-- /About col -->

        <!-- Services col -->

        <div class="col-3 col-sm-6 col-md-3">
          <div class="p-4 bg-dark rounded">
            <div class="text-white">
              <h1 class="fs-4">Services</h1>
              <ul>
                <li><a href="#"> Audit Assurance</a></li>
                <li><a href="#"> Financial Advisory</a></li>
                <li><a href="#"> Analytics MA</a></li>
                <li><a href="#"> Middle MArketing</a></li>
                <li><a href="#"> Legal Consulting</a></li>
                <li><a href="#"> Regularity Risk</a></li>
              </ul>
            </div>
          </div>
        </div>
        <!-- /Services col -->

        <!-- Support col -->

        <div class="col-3 col-sm-6 col-md-3">
          <div class="p-4 bg-dark rounded">
            <div class="text-white">
              <h1 class="fs-4">Support</h1>
              <ul>
                <li><a href="#"> Responsability</a></li>
                <li><a href="#"> Terms of Use</a></li>
                <li><a href="#"> About Cookies</a></li>
                <li><a href="#"> Privacy Policy</a></li>
                <li><a href="#"> Accessibility</a></li>
                <li><a href="#"> Information</a></li>
              </ul>
            </div>
          </div>
        </div>
        <!-- /Support col -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "JumbotronFooter",
  data() {
    return {
      infoLink: [
        {
          title: "About",
          link1: "",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "@/style/mixin";
* {
  margin: 0;
  padding: 0;
}

.jumbotron {
  height: 500px;
  background-image: url("../assets/img/bg-7.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
#logo {
  color: white;

  h1 {
    font-size: 20px;
  }
}

#logo span {
  font-size: 20px;
  padding-left: 30px;
  padding-top: 15px;
  padding-bottom: 15px;
  color: $bg-btn;
  background-color: #52b9bb60;
  border-radius: 40px 0 0 40px;
}
ul {
  list-style: none;
  li {
    line-height: 2rem;
  }
  li a {
    color: #bcbdbd;
    text-decoration: none;
  }
}
</style>
