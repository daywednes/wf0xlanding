<template>
  <div class="main-container wf-container" style="background:#0c1e46;">
    <!-- Navbar section -->
    <NavbarTwo />

    <!-- slider section -->
    <HeroBannerFive />
    <!-- about app -->
    <div class="wf-container">
      <Blog />
      <!-- screenshotTwo section -->
      <ScreenshotTwo />
    </div>
    <!-- <CounterUpTwo /> -->

    <!-- Service style -->
    <Service />

    <!-- Testimonial section -->
    <TestimonialFour testimonialStyle="testimonial-five" />

    <!-- team section -->
    <TeamDoctor />

    <!-- download section -->
    <DownloadFour />

    <!-- policy section -->
    <Policy />

    <!-- call to action -->
    <CallToAction />

    <!-- department section -->
    <Department />

    <!-- google map section -->
    <!-- <GoogleMap /> -->

    <!-- footer section -->
    <FooterTwo />
  </div>
</template>

<script>
import NavbarTwo from "../components/NavbarTwo";
import ScreenshotTwo from "../components/ScreenshotTwo";
import HeroBannerFive from "../components/HeroBannerFive";
// import MedicalInfo from "../components/MedicalInfo";
// import Appointment from "../components/Appointment";
// import CounterUpTwo from "../components/CounterUpTwo";
import Service from "../components/Service";
import TestimonialFour from "../components/TestimonialFour";
import TeamDoctor from "../components/TeamDoctor";
import DownloadFour from "../components/DownloadFour";
import Policy from "../components/Policy";
import CallToAction from "../components/CallToAction";
import Department from "../components/Department";
import Blog from "../components/Blog";
// import GoogleMap from "../components/GoogleMap";
import FooterTwo from "../components/FooterTwo";

export default {
  name: "app",
  components: {
    ScreenshotTwo,
    NavbarTwo,
    HeroBannerFive,
    // MedicalInfo,
    // Appointment,
    // CounterUpTwo,
    Service,
    TestimonialFour,
    TeamDoctor,
    DownloadFour,
    Policy,
    CallToAction,
    Department,
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
