<template>
  <div>
    <div class="container-md p_gioia">
      <!-- Paragrafetto iniziale -->
      <div class="row">
        <div class="col-12">
          <h6 class="font_color py-2"><strong>WE LIKE WHAT WE DO</strong></h6>
        </div>
      </div>
      <!-- /Paragrafetto iniziale -->
      <div class="row">
        <div class="col-8">
          <!-- Titolo e paragrafo di 'Team Experts' -->
          <div class="text-team">
            <h1>
              <strong><span class="bg-opacity">Team</span> of Experts</strong>
            </h1>
            <p>
              Ethics and integrity are the bases on which our professionals
              build their careers. They are fundamentals that become daily
              attitudes.
            </p>
          </div>
          <!-- /Titolo e paragrafo di 'Team Experts' -->
          <!-- Griglia Team -->

          <div class="row g-2">
            <div
              class="col-sm-6 col-md-6 col-6"
              v-for="(item, i) in teams"
              :key="i"
            >
              <div class="row">
                <div class="col-sm-6 col-md-6 col-6">
                  <div class="w-100">
                    <img
                      :src="require(`@/assets/img/${item.image}`)"
                      alt="item"
                      class="w-100 img-fluid b-radius"
                    />
                  </div>
                </div>

                <div class="col-sm-6 col-md-6 col-6 d-flex">
                  <div class="text-teams d-flex flex-column">
                    <h1 class="fs-4 font_weight">{{ item.namePerson }}</h1>
                    <p class="font_size text_color font_weight1">
                      {{ item.job }}
                    </p>
                    <div class="icon-container w-100">
                      <b-icon
                        :icon="icon"
                        v-for="(icon, j) in item.icon"
                        :key="j"
                        style="color: #048383"
                        class="bg-opacity b-radius2"
                        font-scale="3"
                      ></b-icon>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <!-- /Griglia Team -->
        </div>
        <div class="col-4 col-sm-4 col-md-4 bg_btn text-white b-radius">
          <div class="text-president p_20">
            <h1 class="fs-4">President Speech</h1>
            <div class="fs_6">
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Culpa
                harum vitae beatae sed esse tempore ullam, aliquam delectus modi
                excepturi optio nostrum quia qui ab animi magnam aut labore et.
              </p>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Culpa
                harum vitae beatae sed esse tempore ullam, aliquam delectus modi
                excepturi optio nostrum quia qui ab animi magnam aut labore et.
              </p>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Culpa
                harum vitae beatae sed esse tempore ullam, aliquam delectus modi
                excepturi optio nostrum quia qui ab animi magnam aut labore et.
              </p>
            </div>

            <h4>T.Johnson</h4>
          </div>
        </div>
      </div>
    </div>
    <TeamAreaBottom />
  </div>
</template>

<script>
import TeamAreaBottom from "@/components/TeamAreaBottom.vue";
export default {
  name: "TeamArea",
  components: {
    TeamAreaBottom,
  },
  data() {
    return {
      teams: [
        {
          image: "team-1.jpg",
          namePerson: "David Cooper",
          job: "CTO & CO-FOUNDER",
          icon: ["facebook", "twitter", "linkedin"],
        },
        {
          image: "team-3.jpg",
          namePerson: "Oliver Jones",
          job: "CHIEF PROCUREMENT",
          icon: ["facebook", "twitter", "linkedin"],
        },
        {
          image: "team-2.jpg",
          namePerson: "Emma Lopez",
          job: "CHIEF MARKETING",
          icon: ["facebook", "twitter", "linkedin"],
        },
        {
          image: "team-4.jpg",
          namePerson: "T.Johnson",
          job: "CEO PRESIDENT",
          icon: ["facebook", "twitter", "linkedin"],
        },
      ],
    };
  },
};
</script>
<style scoped lang="scss">
.p_20 {
  padding: 20px;
}
.fs_6 {
  font-size: 14px;
}
</style>
