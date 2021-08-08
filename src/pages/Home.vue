<template>
  <div class="main-container">
    <!-- Navbar section -->
    <NavbarTwo />

    <!-- slider section -->
    <HeroBannerFive />
    <div class="wf-container div-shadow">
      <AboutWF />
    </div>
    <section id="feature">
      <div class="wf-container div-shadow">
        <GameTournament />
        <LiveTournament />
      </div>
      <!-- <div class="wf-container2 div-shadow">
      </div> -->
      <!-- <div class="wf-container4 div-shadow"></div> -->
      <div class="wf-container div-shadow">
        <MiniGame />
        <Fusion />
      </div>
    </section>

    <TeamCharacter class="div-shadow" />

    <section id="roadmap" class="wf-container div-shadow">
      <RoadMap />
    </section>

    <section id="tokenView" class="wf-container div-shadow">
      <TokenView />
      <TokenEconmics />
    </section>
    <section id="wfteam" class="wf-container div-shadow">
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
  background-image: url("../assets/img/wf0x/title-pu.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  color: white !important;
  padding: 5px 20px;
  margin: 15px 20%;
  overflow-wrap: anywhere;
  text-align: center;
}

.header-content2 {
  background-image: url("../assets/img/wf0x/l1.png");
  background-position: right;
  background-repeat: no-repeat;
  background-size: cover;
  max-width: 600px;
  /* color: #39a5ff !important; */
  color: white !important;
  padding: 20px;
  font-weight: bold;
  font-size: 42px;
  margin: 50px 0px 30px 0px;
  overflow-wrap: anywhere;
}

/* @media (max-width: 500px) {
  .header-content2 {
    margin-left: 0px;
    font-size: 32px;
  }
} */

.header-detail {
  font-size: x-large;
  /* text-transform: uppercase; */
  font-weight: bold;
  color: #6d6d96;
}
.wf-container {
  background-image: url("../assets/img/wf0x/background-2.png");
  /* background-position: center; */
  background-repeat: no-repeat;
  background-size: cover;
  margin-bottom: 30px;
}
.wf-container2 {
  background-image: url("../assets/img/wf0x/BG3.png");
  /* background-position: center; */
  background-repeat: no-repeat;
  background-size: cover;
  padding-bottom: 30px;
}
.wf-container3 {
  background-image: url("../assets/img/wf0x/BG4.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  margin-bottom: 50px;
}
.wf-container4 {
  background-image: url("../assets/img/wf0x/BG5.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  margin-bottom: 50px;
}

.wf-container5 {
  background-image: url("../assets/img/wf0x/background-team.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.wf-token {
  background-image: url("../assets/img/wf0x/token.png");
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: contain;
  margin-bottom: 50px;
}

.div-shadow {
  -moz-box-shadow: inset 0 0 -20px #0c1e46;
  -webkit-box-shadow: inset 0 0 -20px #0c1e46;
  box-shadow: inset 0 0 -20px #0c1e46;
  margin-bottom: 10px;
  /* padding-bottom: 50px; */
}
</style>
