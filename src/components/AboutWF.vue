<template>
  <div class="screenshot-style-2 bg-cover section live-footer-2">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h1 class="title header-content2">ABOUT FANTASY 0X</h1>
        </div>
      </div>

      <div class="row">
        <div class="col-md-8">
          <div class="text-center">
            <p
              class="header-detail"
              style="padding-bottom: 50px; text-align: left; font-size:x-large;"
            >
              <span><img src="../assets/img/icon/Asset5.png"/></span>
              Fantasy 0x (F0x) is a global fantasy football game where you can
              create your hero team consisting of F0x AI. It will be directly
              related to the performance and abilities of football players in
              the real world.

              <br />
              <br />
              Players can manage their football teams, making them stronger
              through interesting mini-games and functions. By joining great
              tournaments based on live seasons and tournaments, and by relying
              on your smart strategies, you can earn more resources and create
              more real value in this game, as well as during its next phases.
              <span><img src="../assets/img/icon/Asset4.png"/></span>
            </p>
          </div>
        </div>
        <div class="col-md-4">
          <img
            src="../assets/img/wf0x/feature/t2.png"
            alt="doctor thumb"
            style="max-height:600px;"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "GameTournament",
  data() {
    return {
      bgImg: {
        backgroundImage: `url(${require("../assets/img/bg/screenshot-bg.jpg")})`,
      },
      swiperOption: {
        speed: 600,
        loop: true,
        slidesPerView: 3,
        effect: "coverflow",
        // grabCursor: true,
        centeredSlides: true,
        coverflowEffect: {
          rotate: -25,
          stretch: 0,
          depth: 100,
          modifier: 1,
          slideShadows: false,
        },
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
        breakpoints: {
          768: {
            spaceBetween: 60,
          },
          576: {
            slidesPerView: 2,
            spaceBetween: 20,
          },
        },
      },
    };
  },
};
</script>
<style>
.live-footer-2 {
  /* background-image: url("../assets/img/wf0x/hn.png"); */
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: contain;
}
@media (max-width: 500px) {
  .live-footer-2 {
    background-size: contain !important;
  }
}
</style>
