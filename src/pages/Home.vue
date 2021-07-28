<template>
  <div class="main-container wf-container" style="background:#0c1e46;">
    <!-- Navbar section -->
    <NavbarTwo />

    <!-- slider section -->
    <HeroBannerFive />
    <section id="feature" class="wf-container div-shadow">
      <Blog />
      <ScreenshotTwo />
      <MiniGame />
      <Fusion />
    </section>

    <TeamCharacter class="div-shadow" />
    <section id="roadmap" class="wf-container2 div-shadow">
      <FeatureTwo />
    </section>

    <section id="tokenView" class="wf-container4 div-shadow">
      <TokenView />
      <About />
    </section>
    <section id="wfteam" class="wf-container3 div-shadow">
      <WFTeam />
    </section>
    <FooterTwo />
  </div>
</template>

<script>
import NavbarTwo from "../components/NavbarTwo";
import ScreenshotTwo from "../components/ScreenshotTwo";
import MiniGame from "../components/MiniGame";
import Fusion from "../components/Fusion";
import HeroBannerFive from "../components/HeroBannerFive";
import FeatureTwo from "../components/FeatureTwo";
import TeamCharacter from "../components/TeamCharacter";
import Blog from "../components/Blog";
import About from "../components/About";
import WFTeam from "../components/WFTeam";
import TokenView from "../components/TokenView";
import FooterTwo from "../components/FooterTwo";

export default {
  name: "app",
  components: {
    ScreenshotTwo,
    MiniGame,
    Fusion,
    NavbarTwo,
    HeroBannerFive,
    FeatureTwo,
    TeamCharacter,
    Blog,
    About,
    WFTeam,
    TokenView,
    FooterTwo,
  },
};
</script>
<style>
.wf-container {
  background-image: url("../assets/img/wf0x/background-2.png");
  /* background-position: center; */
  background-repeat: no-repeat;
  background-size: cover;
}
.wf-container2 {
  background-image: url("../assets/img/wf0x/BG3.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.wf-container3 {
  background-image: url("../assets/img/wf0x/BG4.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.wf-container4 {
  background-image: url("../assets/img/wf0x/BG5.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
