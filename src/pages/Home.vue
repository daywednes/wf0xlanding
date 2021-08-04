<template>
  <div class="main-container">
    <!-- Navbar section -->
    <NavbarTwo />

    <!-- slider section -->
    <HeroBannerFive />
    <section id="feature">
      <div class="wf-container div-shadow">
        <AboutWF />
        <GameTournament />
      </div>
      <div class="wf-container4 div-shadow">
        <LiveTournament /> <MiniGame />
      </div>
      <div class="wf-container3 div-shadow">
        <Fusion />
      </div>
    </section>

    <TeamCharacter class="div-shadow" />

    <section id="roadmap" class="wf-container2 div-shadow">
      <RoadMap />
    </section>

    <section id="tokenView">
      <TokenView class="wf-container div-shadow" />
      <TokenEconmics class="wf-container4 div-shadow" />
    </section>
    <section id="wfteam" class="wf-container5 div-shadow">
      <WFTeam />
    </section>
    <FooterTwo />
  </div>
</template>

<script>
import NavbarTwo from "../components/NavbarTwo";
import AboutWF from "../components/AboutWF";
import GameTournament from "../components/GameTournament";
import MiniGame from "../components/MiniGame";
import Fusion from "../components/Fusion";
import HeroBannerFive from "../components/HeroBannerFive";
import RoadMap from "../components/RoadMap";
import TeamCharacter from "../components/TeamCharacter";
import LiveTournament from "../components/LiveTournament";
import TokenEconmics from "../components/TokenEconmics";
import WFTeam from "../components/WFTeam";
import TokenView from "../components/TokenView";
import FooterTwo from "../components/FooterTwo";

export default {
  name: "app",
  components: {
    AboutWF,
    GameTournament,
    MiniGame,
    Fusion,
    NavbarTwo,
    HeroBannerFive,
    RoadMap,
    TeamCharacter,
    LiveTournament,
    TokenEconmics,
    WFTeam,
    TokenView,
    FooterTwo,
  },
};
</script>
<style>
.header-content {
  background-image: url("../assets/img/wf0x/title.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  color: white !important;
  padding: 5px 70px;
  margin: 10px 0px;
  max-width: 500px;
  overflow-wrap: anywhere;
}

.header-content2 {
  background-image: url("../assets/img/wf0x/l1.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
  /* color: #39a5ff !important; */
  color: white !important;
  padding: 50px;
  font-weight: bold;
  font-size: 50px;
  overflow-wrap: anywhere;
}

.header-detail {
  font-size: large;
  text-transform: uppercase;
  font-weight: bold;
  color: #696969;
}
.wf-container {
  background-image: url("../assets/img/wf0x/background-2.png");
  /* background-position: center; */
  background-repeat: no-repeat;
  background-size: cover;
}
.wf-container2 {
  background-image: url("../assets/img/wf0x/BG3.png");
  /* background-position: center; */
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

.wf-container5 {
  background-image: url("../assets/img/wf0x/background-team.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

.div-shadow {
  -moz-box-shadow: inset 0 0 -20px #0c1e46;
  -webkit-box-shadow: inset 0 0 -20px #0c1e46;
  box-shadow: inset 0 0 -20px #0c1e46;
  margin-bottom: 15px;
  padding-bottom: 50px;
}
</style>
