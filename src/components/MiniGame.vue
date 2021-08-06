<template>
  <div
    class="latest-blog-area section section-padding  live-footer"
    style="padding-bottom:6%"
  >
    <div class="row">
      <div class="col-12">
        <div>
          <!-- <h1 class="title header-content2">TRAINING</h1> -->
          <div class=" text-center">
            <img
              src="../assets/img/wf0x/feature/training.png"
              alt="doctor thumb"
            />
          </div>

          <div
            class="header-content text-center"
            style="max-width: 100%; margin:30px 20%"
          >
            <h2 style="color:white;overflow-wrap: anywhere;">
              TRAINING
            </h2>
          </div>
          <p class="header-detail text-center" style="color:white;">
            “Users can train robots by joining some mini games. You will need to
            select which robots you want to train, pay certain resources based
            on robots and get attribute increases for selected robots based on
            your result in mini games”
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "LiveTournament",
  data() {
    return {
      blogs: [
        {
          thumb: require("../assets/img/home-medical/blog/1.jpg"),
          date: "14 FEB",
          icon: "fa fa-comment",
          comment: "12",
          title: "Duis autem vel eum iriure dolor.",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum. Typi non habent claritatem insitam.",
          link: "#",
        },
        {
          thumb: require("../assets/img/home-medical/blog/2.jpg"),
          date: "18 JUN",
          icon: "fa fa-comment",
          comment: "32",
          title: "Autem duis vel eum dolor iriure.",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum. Typi non habent claritatem insitam.",
          link: "#",
        },
        {
          thumb: require("../assets/img/home-medical/blog/3.jpg"),
          date: "16 MAR",
          icon: "fa fa-comment",
          comment: "10",
          title: "Iriure duis autem vel eum dolor.",
          desc:
            "Nam liber tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim assum. Typi non habent claritatem insitam.",
          link: "#",
        },
      ],
    };
  },
};
</script>
<style scoped>
.live-div {
  background-image: url("../assets/img/wf0x/feature/training.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
  height: 100%;
  min-height: 500px;
  padding: 250px 20% 0px 20%;
}
</style>
