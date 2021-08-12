<template>
  <section class="feature-style-2 bg-cover section live-footer">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <!-- <div class="header-content">
            <h2 style="color:white;">ROAD MAP</h2>
          </div> -->
          <h1 class="title header-content2">ROAD MAP</h1>
        </div>
      </div>
      <div class="row align-items-center">
        <div class="col-lg-8">
          <div class="feture-thumb">
            <img
              src="../assets/img/wf0x/Ronaldo.gif"
              alt="feature thumb"
              style="max-height:75vh"
            />
          </div>
        </div>
        <div class="col-lg-4">
          <div class="feature-wrapper">
            <div
              v-for="sinFeature in sinFeatures"
              :key="sinFeature.id"
              class="sin-feature fix"
            >
              <!-- <div class="icon">
                <i :class="sinFeature.icon"></i>
              </div> -->
              <div class="content">
                <div class="header-content">
                  <h4 style="color:white;">{{ sinFeature.title }}</h4>
                </div>
                <h5 class="mobile-description text-center">
                  <!-- <span><img src="../assets/img/icon/Asset5.png"/></span> -->
                  {{ sinFeature.desc }}
                  <!-- <span><img src="../assets/img/icon/Asset4.png"/></span> -->
                </h5>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "RoadMap",
  data() {
    return {
      bgImg: {
        backgroundImage: `url(${require("../assets/img/feature-bg.jpg")})`,
      },
      sinFeatures: [
        {
          title: "Q3 2021",
          desc: "Collect & Breeding & Marketplace",
          icon: "fa fa-cogs",
        },
        {
          title: "Q4 2021",
          desc: "Introduce Mini-game Events, Fantasy Tournaments",
          icon: "fa fa-cogs",
        },
        {
          title: "Q1 2022",
          desc: "More Mini-game Events, Launch the Fusion Feature.",
          icon: "fa fa-envelope-o",
        },
        {
          title: "Q3 2022",
          desc: "Introduce League Tournaments.",
          icon: "fa fa-play-circle-o",
        },
        {
          title: "Q4 2022",
          desc: "Introduce Healthcare: Use game tokens to increase stamina.",
          icon: "fa fa-comments",
        },
        {
          title: "Q1 2023",
          desc: "Introduce new robot types & customization options.",
          icon: "fa fa-cloud",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../assets/scss/variables.scss";
@import "../assets/scss/components/feature.scss";
.mobile-description {
  color: #6d6d96 !important;
}
@media (max-width: 500px) {
  .mobile-description {
    // color: white !important;
  }
}
</style>
