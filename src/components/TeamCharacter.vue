<template>
    <section class="team-area section-padding fix section character-bg" id="team">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <!-- <div class="section-title title-style-5 text-center">
                        <h2 class="title">OUR CHARACTERS</h2>
                        <p class="paragraph">Claritas est etiam processus dynamicus, qui sequitur mutationem consuetudium lectorum.</p>
                    </div> -->
                    
            <div class="header-content">
              <h2 style="color:white;">CHARACTERS</h2>
            </div>
                </div>
            </div>
            <div class="row">
                <div class="col-12">
                    <carousel class="doctor-team-carousel"
                        :item = "4"
                        :nav = "false"
                        :dots = "false"
                        :autoplay = "true"
                        :margin = "50"
                        :loop = "true"
                        :smartSpeed = "300"
                        :responsive="{0:{items:1},576:{items:2},768:{items:4}}"
                    >
                        <div v-for="(doctor, doctors) in doctors" :key="doctors" class="doctor-member">
                            <div class="doctor-thumb">
                                <img :src="doctor.thumb" alt="doctor thumb">
                                <div class="doctor-content">
                                    <h6 class="title">{{ doctor.title }}</h6>
                                    <p class="designation">{{ doctor.designation }}</p>
                                </div>
                            </div>
                        </div>
                    </carousel>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    import carousel from 'vue-owl-carousel'
    export default {
        name: 'TeamCharacter',
        components: {
            carousel 
        },
        data (){
            return {
                doctors:[
                    {
                        title: "COMMON ROBOT", 
                        designation: "Deltal Specialist", 
                        thumb: require("../assets/img/wf0x/character/c1.png")
                    },
                    {
                        title: "RARE ROBOT", 
                        designation: "Deltal Specialist", 
                        thumb: require("../assets/img/wf0x/character/c2.png")
                    },
                    {
                        title: "EPIC ROBOT", 
                        designation: "Deltal Specialist", 
                        thumb: require("../assets/img/wf0x/character/c3.png")
                    },
                    {
                        title: "LEGEND ROBOT", 
                        designation: "Deltal Specialist", 
                        thumb: require("../assets/img/wf0x/character/c4.png")
                    }
                ]
            }
        }
    }
</script>

<style lang="scss">
    @import '../assets/scss/variables.scss';
    @import '../assets/scss/components/team.scss';
    .character-bg{
        background-image: url("../assets/img/wf0x/character/bc.png");
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
    }
</style>
