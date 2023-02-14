<script>

export default {
    name: 'AppProcess',
    data() {
        return {
            cards:[
                {
                    link: '/src/assets/img/process1.png',
                    n: 1,
                    title: 'Pre-Production',
                    text: "We'll take your idea and create a technical script which consists of action notes and animation descriptions",
                },
                {
                    link: '/src/assets/img/process2.png',
                    n: 2,
                    title: 'Scripting',
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae libero nulla illum laudantium totam sit excepturi?",
                },
                {
                    link: '/src/assets/img/process1.png',
                    n: 3,
                    title: 'Modelling',
                    text: "Corrupti soluta necessitatibus distinctio adipisci unde quam illo eos rerum recusandae placeat. Lorem Vitae situm grazie.",
                },
                {
                    link: '/src/assets/img/process2.png',
                    n: 4,
                    title: 'Performance',
                    text: "Doloremque eaque vitae hic repellendus, expedita eum rerum esse est impedit veritatis. Dolor sit amet codestum momentum",
                },
            ],
            currentCard: 0,
        }
    },
    methods:{
        gotoPrev() {
          this.currentCard--;
          if (this.currentCard < 0) {
            this.currentCard = this.cards.length - 1;
          }
        },
        gotoNext() {
          this.currentCard++;
          if (this.currentCard == this.cards.length) {
            this.currentCard = 0;
          }
          else if(this.currentCard == 3){
            this.currentCard = 0
          }
          console.log(this.currentCard)
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
    <!-- SECTION PROCESS -->
    <section id="process">
        <!-- CONTAINER PROCESS -->
        <div class="position-relative">
            <!-- THUMB IMAGE PROCESS -->
            <div class="process-thumb">
                <img class="img-fluid"  src="../assets/img/process-thumb.png" alt="process">
            </div>
            <!-- TEXT PROCESS  -->
            <div class="text-section w-50 ms-auto">
                <h5>Our Process</h5>
                <h2>Our Process for</h2>
                <h2>Your Animation</h2>
                <h2>Production</h2>
                <p>We have an effective process for woking on animation</p>
                <!-- CARDS CONTAINER -->
                <div class="d-flex text-center">
                    <!-- CARD PROCESS -->
                    <div class="card card-process py-4 px-3 me-4" :class="{'active-card': index === currentCard},{'active-card': index === currentCard+1}" v-for="card,index in cards">
                        <div class="bg-processimg mx-auto mb-2">
                            <img class="img-fluid"  :src="card.link" alt="process1">
                        </div>
                        <div class="index-process py-4">{{ card.n }}</div>
                        <h1>{{ card.title }}</h1>
                        <p class="mb-0">{{ card.text }}</p>
                    </div>
                </div>
                <!-- BUTTON ARROW PROCESS -->
                <div class="btn-process d-flex mt-3">
                    <div @click="gotoPrev()" class="me-3">
                        <i class="fa-sharp fa-solid fa-arrow-left"></i>
                    </div>
                    <div @click="gotoNext()">
                        <i class="fa-solid fa-arrow-right"></i>
                    </div>
                </div>
                <!-- ROCKET IMG PROCESS -->
                <div class="rocket">
                    <img class="w-50 img-fluid" src="../assets/img/smart4.png" alt="rocket">
                </div>
            </div>





        </div>

    </section>

</template>

<style lang="scss" scoped>

</style>