<template>
  <div class="latest-blog-area live-footer" style="padding-bottom:6%">
    <div class="container" style="height: 100%">
      <div class="row">
        <div class="col-12">
          <h1 class="title header-content2">F0x TOKEN</h1>
          <div class="text-center">
            <img
              src="../assets/img/wf0x/token2.png"
              alt="doctor thumb"
              style="max-height:600px;"
            />
            <!-- <div class="header-content">
              <h2 style="color:white;">F0x TOKEN</h2>
            </div> -->
            <p
              class="header-detail text-center"
              style=" padding:50px; color:white"
            >
              “F0x token is the main in-game currency. It will be used for
              trading, exchanging, improving the Pets and their special
              qualities, mainly in the first phase.”
            </p>
          </div>
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
