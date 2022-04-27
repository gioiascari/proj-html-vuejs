<template>
  <div>
    <div class="container-md py-4">
      <!-- Paragrafetto iniziale -->
      <div class="row">
        <div class="col-12">
          <p>WE LIKE WHAT WE DO</p>
        </div>
      </div>
      <!-- /Paragrafetto iniziale -->
      <div class="row">
        <div class="col-8">
          <!-- Titolo e paragrafo di 'Team Experts' -->
          <div class="text-team">
            <h1>
              <strong><span>Team</span> of Experts</strong>
            </h1>
            <p>
              Ethics and integrity are the bases on which our professionals
              build their careers. They are fundamentals that become daily
              attitudes
            </p>
          </div>
          <!-- /Titolo e paragrafo di 'Team Experts' -->
          <!-- Griglia Team -->

          <div class="row g-2">
            <div class="col-6" v-for="(item, i) in teams" :key="i">
              <div class="row">
                <div class="col-5">
                  <div>
                    <img
                      :src="require(`@/assets/img/${item.image}`)"
                      alt="item"
                      class="w-100"
                    />
                  </div>
                </div>

                <div class="col-7">
                  <div class="text-teams">
                    <h1 class="fs-6">{{ item.namePerson }}</h1>
                    <p class="font_size">{{ item.job }}</p>
                    <b-icon
                      :icon="icon"
                      v-for="(icon, j) in item.icon"
                      :key="j"
                    ></b-icon>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <!-- /Griglia Team -->
        </div>
        <div class="col-4 bg-primary text-white">
          <div class="text-president">
            <h1 class="fs-4">President Speech</h1>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Culpa
              harum vitae beatae sed esse tempore ullam, aliquam delectus modi
              excepturi optio nostrum quia qui ab animi magnam aut labore et.
              beatae sed esse tempore ullam, aliquam delectus modi excepturi
            </p>
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
.font_size {
  font-size: 10px;
}
</style>
