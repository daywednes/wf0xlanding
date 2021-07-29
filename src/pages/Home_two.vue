<template>
    <div class="main-container">

        <!-- Navbar section -->
        <Navbar NavbarStyle="NavbarStyle" />

        <!-- slider section -->
        <HeroBanner />

        <!-- about section -->
        <TokenEconmics AboutStyle="about-style-2" />

        <!-- best app section -->
        <BestappTwo />

        <!-- feature style -->
        <RoadMap />

        <!-- Testimonial section -->
        <TestimonialTwo />

        <!-- screenshotTwo section -->
        <GameTournament />

        <!-- Video section -->
        <VideoTwo />

        <!-- Price section -->
        <Price />

        <!-- Download section -->
        <DownloadTwo />

        <!-- contact section -->
        <Contact ContactStyle="contact-style-2" />

        <!-- footer section -->
        <Footer FooterStyle="footer-style-2" />

    </div>
</template>

<script>
    import Navbar from '../components/Navbar'
    import HeroBanner from '../components/HeroBanner'
    import TokenEconmics from '../components/TokenEconmics'
    import BestappTwo from '../components/BestappTwo'
    import RoadMap from '../components/RoadMap'
    import TestimonialTwo from '../components/TestimonialTwo'
    import GameTournament from '../components/GameTournament'
    import VideoTwo from '../components/VideoTwo'
    import Price from '../components/Price'
    import DownloadTwo from '../components/DownloadTwo'
    import Contact from '../components/Contact'
    import Footer from '../components/Footer'

    export default {
        name: 'app',
        components: {
            Navbar,
            HeroBanner,
            TokenEconmics,
            BestappTwo,
            RoadMap,
            TestimonialTwo,
            GameTournament,
            VideoTwo,
            Price,
            DownloadTwo,
            Contact,
            Footer,
        }
    }
</script>

