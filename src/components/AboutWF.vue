<template>
  <div class="screenshot-style-2 bg-cover section section-padding">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h1 class="title text-center header-content2">ABOUT WF0x</h1>
        </div>
      </div>

      <div class="row">
        <div class="col-12">
          <div class="text-center">
            <p class="header-detail text-center">
              “WORLD FANTASY 0X (WF0X) IS A GLOBAL FANTASY FOOTBALL GAME WHERE
              YOU CAN CREATE YOUR HERO TEAM WITH WF0X ROBOTS. IT WILL INTERACT
              DIRECTLY WITH THE PERFORMANCE AND ABILITY OF FOOTBALL PLAYERS IN
              THE REAL WORLD. MANAGING YOUR OWN FOOTBALL TEAM, MAKING THEM
              STRONGER THROUGHOUT INTERESTING MINI GAMES AND FUNCTIONS. JOINING
              GREAT TOURNAMENTS BASED ON THE LIVE SEASONS AND TOURNAMENTS BASED
              ON YOUR SMART STRATEGIES, YOU CAN EARN MORE RESOURCES AND CREATE
              MORE REAL VALUE IN THIS GAME AS WELL AS THE NEXT PHASES.”
            </p>
          </div>
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
