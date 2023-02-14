<script>

export default {
    name: 'AppHeader',
    data() {
        return {
            visible: false,
        }
    },
    methods: {
        activeslider() {
            this.visible = true;
        },
        stopSlider() {
            this.visible = false;
        },
    }
}

</script>

<template>

    <!-- Header  -->

    <header>

        <!-- Header Container -->

        <div class="container-lg">

            <!-- Header Nav -->

            <nav class="d-flex justify-content-between align-items-center header-container">
                <div>
                    <img class="img-fluid"  src="../assets/img/logo.png" alt="logo">
                </div>
                <div class="h-100">
                    <ul class="d-flex h-100 header-list align-items-center">
                        <li>
                            <a href="">Home</a>
                        </li>
                        <li>
                            <a href="">About Us</a>
                        </li>
                        <li>
                            <a href="">Portfolio</a>
                        </li>
                        <li>
                            <a href="">Our Process</a>
                        </li>
                        <li>
                            <a href="">Pricing</a>
                        </li>
                        <li>
                            <a href="">Blog</a>
                        </li>
                        <li>
                            <a href="">Contact</a>
                        </li>
                        <li>
                            <a href="" class="button btn-back text-dark">Get a Quote</a>
                        </li>
                    </ul>
                </div>
            </nav>
        </div>
    </header>

    <!-- Jumbotron -->

    <section class="jumbo">
        <!-- JUMBO ABSOLUTE ITEMS BACKGROUND -->
        <div class="dots w-100 d-flex position-absolute  justify-content-around">
            <div>
                <img class="img-fluid"  src="../assets/img/dots-left.png" alt="">
            </div>
            <div>
                <img class="img-fluid"  src="../assets/img/dots-right.png" alt="">
            </div>
        </div>
        <div class="mans w-100 d-flex position-absolute justify-content-between">
            <div>
                <img class="img-fluid"  src="../assets/img/left-man.png" alt="">
            </div>
            <div>
                <img class="img-fluid"  src="../assets/img/right-man.png" alt="">
            </div>
        </div>
        <div class="globe-1">
            <img class="img-fluid"  src="../assets/img/globe1.png" alt="globe1">
        </div>
        <div class="globe-3">
            <img class="img-fluid"  src="../assets/img/globe3.png" alt="globe3">
        </div>
        <div class="light">
            <img class="img-fluid"  src="../assets/img/light.png" alt="light">
        </div>
        <div class="globe-2">
            <img class="img-fluid"  src="../assets/img/globe2.png" alt="globe2">
        </div>
        <!-- TEXT CONTAINER -->
        <div class="container-lg">
            <div class="text-center jumbo-text mb-5">
                <h5>Image, Create, Experience</h5>
                <h1>We Animate</h1>
                <h1>Whit Ninja-Like Precision</h1>
                <p>We are a character-driven animation studio striving to make high-quality animations.</p>
                <div>
                    <a href="" class="button btn-back text-dark mx-4">Start a Project</a>
                    <a href="" class="button text-white">Portfolio</a>
                </div>
            </div>
            <div class="middle d-flex justify-content-center position-relative">
                <img class="m-auto" src="../assets/img/middle.png" alt="">
                <div class="play-middle" @click="activeslider()">
                    <i v-show="visible == false" class="fa-solid fa-play"></i>
                </div>
                <div v-show="visible == true" class="slider-middle">
                    <iframe width="700" height="400" src="https://www.youtube.com/embed/8X2kIfS6fb8?autoplay=1"
                        title="YouTube video player" frameborder="0"
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                        allowfullscreen v-if="visible == true"></iframe>
                    <i @click="stopSlider()" class="fa-sharp fa-solid fa-circle-xmark cross-middle"></i>
                </div>
            </div>
            <div class="bottom-shape">
                <img src="../assets/img/bottom-shape.png" alt="bottom-shape">
            </div>
        </div>
    </section>

</template>

<style lang="scss">

</style>