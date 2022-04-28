<template>
  <div class="container-md p_5">
    <!-- Text Adv -->
    <div class="row">
      <div class="col-12 d-flex justify-content-center">
        <div class="text-adv text-center py-3">
          <h6 class="font_color py-2"><strong>INTRODUCTION VIDEO</strong></h6>

          <h2>
            <strong>Advisory <span> Performance</span></strong>
          </h2>
          <p>
            Financial executives nedd to review their strategies, operating
            models and capabilities so their areas can generate sound
            information for better decision making.
          </p>
        </div>
      </div>
    </div>
    <!-- / Text Adv -->
    <div class="row">
      <div class="col-12 d-flex justify-content-center">
        <div class="img-adv w-100">
          <img
            src="../assets/img/video-1.jpg"
            alt="ADV"
            class="w-100 position-relative"
          />
          <div class="icon-play">
            <b-icon
              class="position_absolute"
              icon="play-fill"
              font-scale="7.5"
              variant="success"
            ></b-icon>
            <b-icon
              icon="play-fill"
              font-scale="7.5"
              variant="white"
              class="position_absolute1"
            ></b-icon>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AdvTrailer",
};
</script>

<style lang="scss" scoped>
.font_color {
  color: #52babb;
}
span {
  color: #098081;
  background-color: #52b9bb30;
  padding: 0px 10px 0px 10px;
  border-radius: 5px;
}
.p_5 {
  padding: 10%;
}
.position_absolute {
  position: absolute;
  top: 70.5rem;
  left: 47%;
  opacity: 0.6;
}
.position_absolute1 {
  position: absolute;
  top: 71rem;
  left: 47%;
  opacity: 0.7;
}
</style>
