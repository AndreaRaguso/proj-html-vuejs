<script>

export default {
    name: 'AppTeam',
    data() {
        return {
            teams: [
                {
                    link: '/src/assets/img/team1.png',
                    name: 'Robert Coleman',
                    work: 'Owner & Creative Director',
                },
                {
                    link: '/src/assets/img/team2.png',
                    name: 'Don Woods',
                    work: 'Owner & Creative Director',
                },
                {
                    link: '/src/assets/img/team4.png',
                    name: 'Tomas Nash',
                    work: 'Owner & Creative Director',
                },
                {
                    link: '/src/assets/img/team3.png',
                    name: 'Andrea Raguso',
                    work: 'Capo supremo & Milionario',
                },
            ],
            currentTeam: 0,
        }
    },
    methods:{
        gotoPrev() {
          this.currentTeam--;
          if (this.currentTeam < 0) {
            this.currentTeam = this.teams.length - 1;
          }
        },
        gotoNext() {
          this.currentTeam++;
          if (this.currentTeam == this.teams.length) {
            this.currentTeam = 0;
          }
        },

        timingimage(){
            this.play = setInterval(this.gotoNext, 3000);
        }
    },
    mounted(){
        this.timingimage()
    }
}

</script>

<template>

    <!-- SECTION TEAMS -->
    <section id="team" class=" position-relative">
        <!-- SHAPES BACKGROUND TEAMS -->
        <div class="position-absolute">
            <img class="img-fluid"  src="../assets/img/shape.png" alt="">
        </div>
        <div class="position-absolute shape2">
            <img class="img-fluid"  src="../assets/img/shape2.png" alt="">
        </div>
        <!-- TEAMS CONTAINER -->
        <div class="container-lg">
            <!-- TEXT TEAMS CONTAINER -->
            <div class="text-section text-center mx-auto mb-3">
                <h5>Anido Magic Team Member</h5>
                <h2>Let Us Animate Your Project</h2>
                <p>We create new worlds! Let's collaborate and create engaging, effective, award-winning animations</p>
            </div>
            <!-- TEAMS CARDS CONTAINER -->
            <div class="cards-team d-flex justify-content-center">
                <!-- SINGLE CARD -->
                <div class="card-team text-center me-3" v-for="team,index in teams" :class="{'d-none': index === currentTeam}">
                    <div class="team-img">
                        <img class="img-fluid"  :src="team.link" alt="team 1">
                    </div>
                    <div class="team-info">
                        <h5 class=" fw-bold">{{ team.name }}</h5>
                        <p>{{ team.work }}</p>
                    </div>
                    <div class="socials d-flex justify-content-center mb-3">
                        <a href="#"><i class="fab fa-facebook-square fa-2x logo me-3"></i></a>
                        <a href="#"><i class="fab fa-twitter fa-2x logo me-3"></i></a>
                        <a href="#"><i class="fab fa-instagram fa-2x logo"></i></a>
                    </div>
                </div>
            </div>
            <!-- ARROW DOTS CONTAINER -->
            <div class="d-flex mt-4 align-items-center justify-content-center">
                <!-- RIGHT ARROW -->
                <div class="me-3 btn-team" @click="gotoPrev">
                    <i class="fa-sharp fa-solid fa-arrow-left"></i>
                </div>
                <!-- DOTS -->
                <div class="dot-team">
                    <i class="fa-solid fa-circle me-3" v-for="i in teams.length" :class="{'active': i === currentTeam+1}"></i>
                </div>
                <!-- LEFT ARROW -->
                <div class="btn-team ms-3" @click="gotoNext">
                    <i class="fa-solid fa-arrow-right"></i>
                </div>
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>

</style>