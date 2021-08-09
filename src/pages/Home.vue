<template>
  <div class="main-container">
    <!-- Navbar section -->
    <FantasyNavbar />

    <!-- slider section -->
    <FantasyHeroBanner />
    <div class="wf-container2 div-shadow">
      <AboutWF class="wf-container4" />
    </div>
    <section id="feature">
      <div class="wf-container3 div-shadow">
        <GameTournament class="wf-container4" />
      </div>
      <div class="div-shadow">
        <LiveTournament class="wf-container4" />
      </div>
      <!-- <div class="wf-container2 div-shadow">
      </div> -->
      <!-- <div class="wf-container4 div-shadow"></div> -->
      <div class="wf-container3 div-shadow">
        <MiniGame />
      </div>
      s
      <Fusion class="wf-container4" />
    </section>

    <div class="wf-container3 div-shadow">
      <TeamCharacter class="div-shadow wf-container4" />
    </div>

    <section id="roadmap" class="wf-container5 div-shadow">
      <RoadMap />
    </section>

    <section id="tokenView">
      <div class="wf-container4 div-shadow">
        <TokenView />
      </div>
      <div class="wf-container3 div-shadow">
        <TokenEconmics />
      </div>
    </section>
    <section id="wfteam" class="wf-container3 div-shadow">
      <WFTeam class="wf-container4" />
    </section>
    <FantasyFooter />
  </div>
</template>

<script>
import FantasyNavbar from "../components/FantasyNavbar";
import AboutWF from "../components/AboutWF";
import GameTournament from "../components/GameTournament";
import MiniGame from "../components/MiniGame";
import Fusion from "../components/Fusion";
import FantasyHeroBanner from "../components/FantasyHeroBanner";
import RoadMap from "../components/RoadMap";
import TeamCharacter from "../components/TeamCharacter";
import LiveTournament from "../components/LiveTournament";
import TokenEconmics from "../components/TokenEconmics";
import WFTeam from "../components/WFTeam";
import TokenView from "../components/TokenView";
import FantasyFooter from "../components/FantasyFooter";

export default {
  name: "app",
  components: {
    AboutWF,
    GameTournament,
    MiniGame,
    Fusion,
    FantasyNavbar,
    FantasyHeroBanner,
    RoadMap,
    TeamCharacter,
    LiveTournament,
    TokenEconmics,
    WFTeam,
    TokenView,
    FantasyFooter,
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
  background-image: url("../assets/img/wf0x/l2.png");
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
  padding: 20px;
  padding: 0px 8%;
}
.wf-container {
  background-image: url("../assets/img/bg/screenshot-bg.jpg");
  /* background-image: url("../assets/img/wf0x/BG3.png"); */
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  margin-bottom: 30px;
}
.wf-container2 {
  /* background-image: url("../assets/img/wf0x/BG3.png"); */
  background-image: url("../assets/img/wf0x/Asset/Asset111.png");
  /* background-position: center; */
  background-repeat: no-repeat;
  background-size: contain;
  padding-bottom: 30px;
}
.wf-container3 {
  /* background-image: url("../assets/img/wf0x/BG4.png"); */
  background-image: url("../assets/img/wf0x/Asset/Asset6.png");
  background-position: left;
  background-repeat: no-repeat;
  background-size: contain;
  margin-bottom: 50px;
}
.wf-container4 {
  /* background-image: url("../assets/img/wf0x/BG4.png"); */
  background-image: url("../assets/img/wf0x/Asset/Asset31.png");
  background-position: right;
  background-repeat: no-repeat;
  background-size: contain;
  margin-bottom: 50px;
}

.wf-container5 {
  background-image: url("../assets/img/wf0x/Asset/Asset2.png");
  background-position: left;
  background-repeat: no-repeat;
  background-size: contain;
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
