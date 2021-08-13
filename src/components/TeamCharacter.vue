<template>
  <section class="team-area fix section wf-container" id="character">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <!-- <div class="header-content">
            <h2 style="color:white;">CHARACTERS</h2>
          </div> -->

          <h1 class="title header-content2">CHARACTERS</h1>
        </div>
      </div>
      <div class="row">
        <div class="col-12">
          <carousel
            class="doctor-team-carousel character-bg"
            style="padding: 10% 0;"
            :item="5"
            :nav="false"
            :dots="false"
            :autoplay="true"
            :margin="40"
            :loop="true"
            :responsive="{
              0: { items: 1 },
              576: { items: 3 },
              768: { items: 3 },
            }"
          >
            <div
              v-for="(doctor, doctors) in doctors"
              :key="doctors"
              class="doctor-member"
            >
              <div class="doctor-thumb">
                <img
                  :src="doctor.thumb"
                  alt="doctor thumb"
                  style="max-height:900px;max-width:180px; margin: auto;"
                />
                <div class="doctor-content">
                  <h6 class="title">{{ doctor.title }}</h6>
                  <p class="designation">{{ doctor.designation }}</p>
                </div>
              </div>
            </div>
          </carousel>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import carousel from "vue-owl-carousel";
export default {
  name: "TeamCharacter",
  components: {
    carousel,
  },
  data() {
    return {
      doctors: [
        {
          title: "COMMON ROBOT",
          designation: "Deltal Specialist",
          thumb: require("../assets/img/wf0x/character/Asset24.png"),
        },
        {
          title: "RARE ROBOT",
          designation: "Deltal Specialist",
          thumb: require("../assets/img/wf0x/character/Asset21.png"),
        },
        {
          title: "EPIC ROBOT",
          designation: "Deltal Specialist",
          thumb: require("../assets/img/wf0x/character/Asset22.png"),
        },
        {
          title: "LEGEND ROBOT",
          designation: "Deltal Specialist",
          thumb: require("../assets/img/wf0x/character/Asset23.png"),
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../assets/scss/variables.scss";
@import "../assets/scss/components/team.scss";
.character-bg {
  background-image: url("../assets/img/wf0x/Asset18.png");
  background-position: top;
  background-repeat: no-repeat;
  background-size: auto;
}
</style>
