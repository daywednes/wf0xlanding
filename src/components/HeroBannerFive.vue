<template>
  <section
    class="slider-section slider-style-5 section bgimg div-shadow"
    id="home"
  >
    <div class="container">
      <div class="row">
        <div class="col-12">
          <carousel
            class="hero-carousel"
            :items="1"
            :nav="false"
            :dots="false"
            :loop="true"
            :autoplay="true"
          >
            <!-- single slider item -->
            <div
              v-for="(slider, sliders) in sliders"
              :key="sliders"
              class="hero-slider-item"
            >
              <div class="row align-items-center">
                <div class="col-xl-5 col-lg-5 col-md-5">
                  <div class="slider-content">
                    <div class="slider-title">
                      <img :src="slider.logo" alt="slider logo" />
                    </div>
                    <!-- <h6 class="slider-subtitle">{{ slider.subtitle }}</h6>
                    <h2 class="slider-title">{{ slider.sliderTitle }}</h2>
                    <p class="slider-desc">{{ slider.sliderDesc }}</p>
                    <div class="slider-btn">
                      <a href="#" class="btn btn-round">LEARN MORE</a>
                    </div> -->
                  </div>
                </div>
                <div class="col-xl-7 col-lg-7 col-md-7  d-none d-md-block">
                  <div class="slider-thumb">
                    <img :src="slider.sliderThumb" alt="slider thumb" />
                  </div>
                </div>
              </div>
            </div>
            <!-- single slider end -->
          </carousel>
          <!-- <div>
            <div class="header-content">
              <h2 style="color:white;">ABOUT WF0x</h2>
            </div>

            <p class="header-detail text-center">
              “World fantasy 0x (WF0x) is a global fantasy football game where
              you can create your hero team with WF0x robots. It will interact
              directly with the performance and ability of football players in
              the real world. <br />
              Managing your own football team, making them stronger throughout
              interesting mini games and functions. Joining great tournaments
              based on the live seasons and tournaments based on your smart
              strategies, you can earn more resources and create more real value
              in this game as well as the next phases.”
            </p>
          </div> -->
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import carousel from "vue-owl-carousel";
export default {
  name: "HeroBannerFive",
  components: {
    carousel,
  },
  data() {
    return {
      bgImg: {
        backgroundImage: `url(${require("../assets/img/wf0x/background1.png")})`,
        width: `100%`,
      },
      sliders: [
        {
          sliderThumb: require("../assets/img/wf0x/heroimg/char1.png"),
          logo: require("../assets/img/wf0x/logo.png"),
          subtitle: "THE BEST HOSPITALITY VUE TEMPLATE FOREVER!",
          sliderTitle: "FANTASIC HEALTH SYSTEM",
          sliderDesc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.",
        },
        {
          sliderThumb: require("../assets/img/wf0x/heroimg/char2.png"),
          logo: require("../assets/img/wf0x/logo.png"),
          subtitle: "THE BEST HOSPITALITY VUE TEMPLATE FOREVER!",
          sliderTitle: "FANTASIC HEALTH SYSTEM",
          sliderDesc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.",
        },
        {
          sliderThumb: require("../assets/img/wf0x/heroimg/char3.png"),
          logo: require("../assets/img/wf0x/logo.png"),
          subtitle: "THE BEST HOSPITALITY VUE TEMPLATE FOREVER!",
          sliderTitle: "FANTASIC HEALTH SYSTEM",
          sliderDesc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.",
        },
        {
          sliderThumb: require("../assets/img/wf0x/heroimg/char4.png"),
          logo: require("../assets/img/wf0x/logo.png"),
          subtitle: "THE BEST HOSPITALITY VUE TEMPLATE FOREVER!",
          sliderTitle: "FANTASIC HEALTH SYSTEM",
          sliderDesc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum.",
        },
      ],
    };
  },
};
</script>

<style>
.bgimg {
  background-image: url("../assets/img/wf0x/background1.png");
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
