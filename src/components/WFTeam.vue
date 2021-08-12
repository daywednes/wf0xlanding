<template>
  <section class="section" :class="AboutStyle">
    <div class="container">
      <h1 class="title header-content2">TEAM</h1>
      <!-- <div class="header-content">
        <h2 style="color:white;">TEAM</h2>
      </div> -->
      <div class="row" 
            style="padding-bottom: 10%;">
        <!-- single item start -->
        <div
          v-for="(about, abouts) in abouts"
          :key="abouts"
          class="col-lg-3 col-md-6"
        >
          <div class="about-item">
            <img :src="about.img" style="max-height:200px;" />
            <div class="about-content">
              <!-- <h6 style="color:#39a5ff; font-size: large;">
                {{ about.title }}
              </h6>
              <p style="color:white; font-size: large;">{{ about.desc }}</p>
               -->
              <div class="header-content" style="margin:10px;">
                <h4 style="color:white; ">{{ about.title }}</h4>
              </div>
              <h5 class="team-desc text-center">
                {{ about.desc }}
              </h5>
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
          title: "Binh Doan",
          desc: "Project Manager \n",
          icon: "fa fa-pagelines",
          img: require("../assets/img/wf0x/team/BinhDoan.jpg"),
        },
        {
          title: "Vu Hoang",
          desc: "Technical Lead \n" + "Web Developer \n",
          icon: "fa fa-laptop",
          img: require("../assets/img/wf0x/team/VuHN.jpg"),
        },
        {
          title: "Lam Tung La",
          desc: "Game Designer \n" + " \n",
          icon: "fa fa-apple",
          img: require("../assets/img/wf0x/team/LamLT.jpg"),
        },
        {
          title: "Hieu Nguyen",
          desc: "Game Producer \n" + "Game Developer \n" + "@ncc.asia",
          icon: "fa fa-paint-brush",
          img: require("../assets/img/wf0x/team/HieuNguyen.jpeg"),
        },
        {
          title: "Cong Nguyen",
          desc: "Game Developer \n" + " \n" + "@ncc.asia",
          icon: "fa fa-pagelines",
          img: require("../assets/img/wf0x/team/CongNT.jpeg"),
        },
        {
          title: "Trung Hoang",
          desc: "Game Developer \n" + " \n" + "@ncc.asia",
          icon: "fa fa-laptop",
          img: require("../assets/img/wf0x/team/HoangTrung.jpg"),
        },
        {
          title: "Anh Do",
          desc: "Artist \n" + " \n" + "@ncc.asia",
          icon: "fa fa-laptop",
          img: require("../assets/img/wf0x/team/TuanAnh.png"),
        },
        {
          title: "Minh Doan",
          desc: "Advisor \n" + "Genesisbuilders  \n" + "Incubator",
          icon: "fa fa-apple",
          img: require("../assets/img/wf0x/team/MinhDoan.jpg"),
        },
        // {
        //   title: "UNIQUE DESIGN",
        //   desc:
        //     "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet.",
        //   icon: "fa fa-paint-brush",
        //   img: require("../assets/img/wf0x/team/team-avar.png"),
        // },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../assets/scss/variables.scss";
@import "../assets/scss/components/about.scss";

.team-desc {
  color: #6D6D96;
  white-space: pre-line;
  border-top-style: double;
  border-bottom-style: double;
  min-height: 130px;
}
</style>
