<template>
  <section
    class="slider-section slider-style-5 section bgimg2 div-shadow"
    id="home"
  >
    <div class="container">
      <div class="row">
        <div class="col-12 text-center">
          <!-- <button class="submit-btn play-btn" @click="goTo('/coming-soon')">
            Play
          </button> -->
          <img
            style="max-height: 40vh; margin-top: 40vh;"
            src="../assets/img/wf0x/F0x_Logo_Final.png"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import carousel from "vue-owl-carousel";
export default {
  name: "FantasyHeroBanner",
  components: {
    carousel,
  },
  data() {
    return {
      bgImg: {
        backgroundImage: `url(${require("../assets/img/wf0x/background1.png")})`,
        width: `100%`,
      },
    };
  },
  methods: {
    goTo: function(url) {
      this.$router.push(url);
    },
  },
};
</script>

<style>
.bgimg {
  /* background-image: url("../assets/img/wf0x/thu-nghiem.png"); */
  background-image: url("../assets/img/wf0x/background1.png");
  background-position: initial;
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
}
.bgimg2 {
  background-image: url("../assets/img/wf0x/Logo&Banner.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 85vh;
}
</style>
