<template>
  <section
    class="feature-style-2 bg-cover section live-footer"
    style="padding-bottom:15%"
  >
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
              src="../assets/img/wf0x/character/live-tournament.png"
              alt="feature thumb"
              style="max-height:80vh"
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
                <h5 class="mobile-description">
                  {{ sinFeature.desc }}
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
          title: "Q4 2021",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-cogs",
        },
        {
          title: "Q2 2022",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-envelope-o",
        },
        {
          title: "Q3 2022",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-play-circle-o",
        },
        {
          title: "Q1 2023",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-comments",
        },
        {
          title: "Q4 2023",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
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
  color: #696969 !important;
}
@media (max-width: 500px) {
  .mobile-description {
    color: white !important;
  }
}
</style>
