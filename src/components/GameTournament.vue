<template>
  <div class="screenshot-style-2 bg-cover section">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h1 class="title text-center header-content2">FEATURE</h1>
          <br />
          <div class="screenshot-gallery text-center">
            <swiper :options="swiperOption">
              <swiper-slide>
                <div class="scr-thumb">
                  <img
                    src="../assets/img/wf0x/feature/t1.png"
                    alt="screenshot thumb"
                  />
                </div>
              </swiper-slide>
              <swiper-slide>
                <div class="scr-thumb">
                  <img
                    src="../assets/img/wf0x/feature/t2.png"
                    alt="screenshot thumb"
                  />
                </div>
              </swiper-slide>
              <!-- Optional controls -->
              <div class="swiper-button-prev" slot="button-prev"></div>
              <div class="swiper-button-next" slot="button-next"></div>
            </swiper>
          </div>
        </div>
      </div>

      <div class="row">
        <div class="col-12">
          <div class="text-center">
            <div class="header-content">
              <h2 style="color:white;">GAME TOURNAMENT</h2>
            </div>
            <p class="header-detail text-center">
              “Game tournament is win-lose by game formula(addition current
              performance if any). There are weekly, monthly, world tournaments
              and grouping users in different groups based on their strength.”
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
