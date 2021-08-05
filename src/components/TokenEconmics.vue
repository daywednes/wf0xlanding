<template>
  <section class="section" :class="AboutStyle" style="padding-bottom: 100px;">
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
            <img :src="about.img" style="max-height: 350px;" />
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
          title: "In-game Currency",
          desc: "Most items in the game will be payable using F0x tokens.",
          icon: "fa fa-pagelines",
          img: require("../assets/img/wf0x/token/tk1.png"),
        },
        {
          title: "Governance",
          desc:
            "Vote for new features and settings of the game to earn special rewards. Lock F0x tokens for a certain time to gain voting power.",
          icon: "fa fa-laptop",
          img: require("../assets/img/wf0x/token/tk2.png"),
        },
        {
          title: "Staking",
          desc:
            "Become part of the game by staking F0x tokens into pools. Different pools will yield different returns such as new items, new rbots, or F0x tokens.",
          icon: "fa fa-apple",
          img: require("../assets/img/wf0x/token/tk3.png"),
        },
        {
          title: "Play 2 Earn",
          desc:
            "Simply playing can also get you F0x tokens via mission and social mining.",
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
