<template>
  <div class="jumbotron bg-black">
    <div class="container-md p-4">
      <div class="row g-4 py-5 align-items-center">
        <!-- Colonna Logo e icone -->
        <div class="col-3 col-md-3">
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
              <ul>
                <li
                  class="p-2 text_color"
                  v-for="(contact, i) in contacts"
                  :key="i"
                >
                  <i :class="contact.icon"></i>
                  {{ contact.info }}
                </li>
              </ul>
            </div>

            <button class="btn btn_hover" type="submit">GET IN TOUCH</button>
          </div>
        </div>
        <!-- /Colonna Logo e icone -->

        <!-- About col -->
        <div class="col-3 col-md-3" v-for="(item, i) in infoLink" :key="i">
          <div class="p-4 bg_dark rounded">
            <div class="text-white">
              <h1 class="fs-4">{{ item.title }}</h1>
              <ul>
                <div>
                  <li v-for="(service, j) in item.about" :key="j">
                    <a href="#"
                      ><i class="bi bi-chevron-right"></i> {{ service }}</a
                    >
                  </li>
                </div>
              </ul>
            </div>
          </div>
        </div>
        <!-- /About col -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "JumbotronFooter",
  props: ["contacts"],
  data() {
    return {
      infoLink: [
        {
          title: "About",
          about: [
            "The Company",
            "Insitutional",
            "Social & Events",
            "Innovation",
            "Environment",
            "Technology",
          ],
        },
        {
          title: "Services",
          about: [
            "Audit & Assurance",
            "Financial Advisory",
            "Middle MArketing",
            "Innovation",
            "Legal Consulting",
            "Regularity Risk",
          ],
        },
        {
          title: "Support",
          about: [
            "Responsability",
            "Terms of Use",
            "About Cookies",
            "Privacy Policy",
            "Accessibility",
            "Information",
          ],
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
.p_5 {
  padding: 5px;
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

.bg_dark {
  background-color: $bg-card-footer;
  background-blend-mode: multiply;
  background-color: rgba(59, 59, 59, 0.3);
}
</style>
