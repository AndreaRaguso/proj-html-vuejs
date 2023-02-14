<script>

export default {
    name: 'AppWhy',
    data() {
        return {
            images: [
                { link: '/src/assets/img/sponsor1.png' },
                { link: '/src/assets/img/sponsor2.png' },
                { link: '/src/assets/img/sponsor3.png' },
                { link: '/src/assets/img/sponsor4.png' },
                { link: '/src/assets/img/sponsor5.png' },
            ],
            play: undefined,
            currentImage: 0,
        }
    },
    methods:{
        gotoNext() {
          this.currentImage++;
          if (this.currentImage === this.images.length) {
            this.currentImage = 0;
          }
        },

        timingimage(){
            this.play = setInterval(this.gotoNext, 1000);
        }
    },
    mounted(){
        this.timingimage()
    }
}

</script>

<template>

    <!-- WHY SECTIONS -->
    <section id="why">
        <!-- WHY CONTAINER -->
        <div class=" container-lg">
            <!-- TEXT WHY CONTAINER -->
            <div class="text-section mx-auto text-center">
                <h5>Why Anidio studio?</h5>
                <h1>We Love Our Clients</h1>
                <p>We are trusted throughout adiand and have a wealth of recommendations from start-ups to renowned
                    blobal brands.</p>
            </div>
            <!-- SPONSOR IMAGES -->
            <div class="d-flex justify-content-center">
                <div v-for="image,index in images">
                    <img :src="image.link" :class="{'active-sponsor': index === currentImage}" class="me-3 img-fluid" alt="">
                </div>
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>

</style>