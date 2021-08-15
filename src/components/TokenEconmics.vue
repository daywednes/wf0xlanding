<template>
  <section class="section" :class="AboutStyle" style="padding-bottom: 100px;">
    <div class="container">
      <!-- <div class="header-content">
        <h2 style="color:white;">TOKEN ECONOMICS</h2>
      </div> -->
      <h1 class="title header-content2">TOKEN ECONOMICS</h1>
      <div class="row">
        <!-- single item start -->
        <div
          v-for="(about, abouts) in abouts"
          :key="abouts"
          class="col-lg-3 col-md-6"
        >
          <div class="about-item">
            <img :src="about.img" style="height: 300px; margin: auto" />
            <div class="about-content">
              <div class="header-content">
                <h4 style="color:white; ">{{ about.title }}</h4>
              </div>
              <h5 style="color:#6D6D96;margin: 0 15%">{{ about.desc }}</h5>
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
          desc:
            "Most items and actions in the game will be carried out using game token (collect, breed, fusion, enter special events)",
          icon: "fa fa-pagelines",
          img: require("../assets/img/wf0x/token/tk1.png"),
        },
        {
          title: "Governance Token",
          desc:
            "Vote for new features and settings of the game to receive special awards",
          icon: "fa fa-laptop",
          img: require("../assets/img/wf0x/token/tk2.png"),
        },
        {
          title: "Play To Earn Game",
          desc: "Receive tokens via in-game mission and social mining",
          icon: "fa fa-paint-brush",
          img: require("../assets/img/wf0x/token/tk4.png"),
        },
        {
          title: "Staking Token",
          desc:
            "Become part of the game by staking tokens in to pools. Pools allow you to yield new items, gain power, and generate new events",
          icon: "fa fa-apple",
          img: require("../assets/img/wf0x/token/tk3.png"),
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
