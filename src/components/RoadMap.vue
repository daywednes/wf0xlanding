<template>
  <section class="feature-style-2 bg-cover section">
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
            <img src="../assets/img/wf0x/roadmap.png" alt="feature thumb" />
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
                <h5 style="color:#696969">{{ sinFeature.desc }}</h5>
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
          title: "ADVANCED SETTINGS",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-cogs",
        },
        {
          title: "MESSAGES INBOX",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-envelope-o",
        },
        {
          title: "MEDIA PLAYER",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-play-circle-o",
        },
        {
          title: "LIVE CHAT MESSAGES",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-comments",
        },
        {
          title: "WEATHER ON-THE-GO",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-cloud",
        },
        {
          title: "FRIENDS LIST",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-user-plus",
        },
        {
          title: "EVENTS CALENDAR",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-calendar-check-o",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../assets/scss/variables.scss";
@import "../assets/scss/components/feature.scss";
</style>
