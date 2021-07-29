<template>
  <div class="main-container wf-container" style="background:#0c1e46;">
    <!-- Navbar section -->
    <NavbarTwo />

    <!-- slider section -->
    <HeroBannerFive />
    <section id="feature" class="wf-container div-shadow">
      <LiveTournament />
      <GameTournament />
      <MiniGame />
      <Fusion />
    </section>

    <TeamCharacter class="div-shadow" />
    
    <section id="roadmap" class="wf-container div-shadow">
      <RoadMap />
    </section>

    <section id="tokenView" class="wf-container4 div-shadow">
      <TokenView />
      <TokenEconmics />
    </section>
    <section id="wfteam" class="wf-container3 div-shadow">
      <WFTeam />
    </section>
    <FooterTwo />
  </div>
</template>

<script>
import NavbarTwo from "../components/NavbarTwo";
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

.div-shadow {
  -moz-box-shadow: inset 0 0 -20px #0c1e46;
  -webkit-box-shadow: inset 0 0 -20px #0c1e46;
  box-shadow: inset 0 0 -20px #0c1e46;
}
</style>
