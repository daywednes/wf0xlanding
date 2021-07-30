<template>
  <section class=" section" :class="AboutStyle">
    <div class="container">
      <!-- <div class="header-content">
        <h2 style="color:white;">TOKEN ECONOMICS</h2>
      </div> -->
      <h1 class="title text-center header-content2">TOKEN ECONOMICS</h1>
      <div class="row">
        <!-- single item start -->
        <div
          v-for="(about, abouts) in abouts"
          :key="abouts"
          class="col-lg-6 col-md-6"
        >
          <div class="about-item">
            <img :src="about.img" />
            <div class="about-content">
              <div class="header-content">
                <h4 style="color:white;">{{ about.title }}</h4>
              </div>
              <h5 style="color:#696969;">{{ about.desc }}</h5>
            </div>
          </div>
        </div>
        <!-- single item end -->
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "TokenEconmics",
  props: ["AboutStyle"],
  data() {
    return {
      abouts: [
        {
          title: "BUILD SHOWCASE",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-pagelines",
          img: require("../assets/img/wf0x/token/tk1.png"),
        },
        {
          title: "FULL RESPONSIVE",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-laptop",
          img: require("../assets/img/wf0x/token/tk2.png"),
        },
        {
          title: "RETINA READY",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-apple",
          img: require("../assets/img/wf0x/token/tk3.png"),
        },
        {
          title: "UNIQUE DESIGN",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
          icon: "fa fa-paint-brush",
          img: require("../assets/img/wf0x/token/tk4.png"),
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../assets/scss/variables.scss";
@import "../assets/scss/components/about.scss";
</style>
