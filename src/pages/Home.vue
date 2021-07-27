<template>
  <div class="main-container wf-container" style="background:#0c1e46;">
    <!-- Navbar section -->
    <NavbarTwo />

    <!-- slider section -->
    <HeroBannerFive />
    <!-- about app -->
    <section id="blog" class="wf-container">
      <Blog />
      <!-- screenshotTwo section -->
      <ScreenshotTwo />
      <MiniGame />
      <Fusion />
    </section>
    <!-- <CounterUpTwo /> -->
    <!-- team character -->
    <TeamCharacter />

    <!-- Service style -->
    <!-- <Service /> -->
    <FeatureTwo />



    <!-- Testimonial section -->
    <!-- <TestimonialFour testimonialStyle="testimonial-five" /> -->

    <!-- download section -->
    <!-- <DownloadFour /> -->

    <!-- policy section -->
    <!-- <Policy /> -->


    <!-- google map section -->
    <!-- <GoogleMap /> -->

    <!-- footer section -->
    <FooterTwo />
  </div>
</template>

<script>
import NavbarTwo from "../components/NavbarTwo";
import ScreenshotTwo from "../components/ScreenshotTwo";
import MiniGame from "../components/MiniGame";
import Fusion from "../components/Fusion";
import HeroBannerFive from "../components/HeroBannerFive";
// import MedicalInfo from "../components/MedicalInfo";
// import Appointment from "../components/Appointment";
// import CounterUpTwo from "../components/CounterUpTwo";
// import Service from "../components/Service";
import FeatureTwo from "../components/FeatureTwo";
// import TestimonialFour from "../components/TestimonialFour";
import TeamCharacter from "../components/TeamCharacter";
// import DownloadFour from "../components/DownloadFour";
// import Policy from "../components/Policy";
import Blog from "../components/Blog";
// import GoogleMap from "../components/GoogleMap";
import FooterTwo from "../components/FooterTwo";

export default {
  name: "app",
  components: {
    ScreenshotTwo,
    MiniGame,
    Fusion,
    NavbarTwo,
    HeroBannerFive,
    // MedicalInfo,
    // Appointment,
    // CounterUpTwo,
    // Service,
    FeatureTwo,
    // TestimonialFour,
    TeamCharacter,
    // DownloadFour,
    // Policy,
    Blog,
    // GoogleMap,
    FooterTwo,
  },
};
</script>
<style scoped>
.wf-container {
  background-image: url("../assets/img/wf0x/background-2.png");
  /* background-position: center; */
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
