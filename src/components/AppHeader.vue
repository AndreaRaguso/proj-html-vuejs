<script>

export default {
    name: 'AppHeader',
    data() {
        return {
            
        }
    },
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
                    <img src="../assets/img/logo.png" alt="logo">
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
        <div class="dots w-100 d-flex position-absolute  justify-content-around">
            <div>
                <img src="../assets/img/dots-left.png" alt="">
            </div>
            <div>
                <img src="../assets/img/dots-right.png" alt="">
            </div>
        </div>
        <div class="mans w-100 d-flex position-absolute justify-content-between">
            <div>
                <img src="../assets/img/left-man.png" alt="">
            </div>
            <div>
                <img src="../assets/img/right-man.png" alt="">
            </div>
        </div>
        <div class="globe-1">
            <img src="../assets/img/globe1.png" alt="globe1">
        </div>
        <div class="globe-3">
            <img src="../assets/img/globe3.png" alt="globe3">
        </div>
        <div class="light">
            <img src="../assets/img/light.png" alt="light">
        </div>
        <div class="globe-2">
            <img src="../assets/img/globe2.png" alt="globe2">
        </div>
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
            <div class="middle d-flex justify-content-center">
                <img class="m-auto" src="../assets/img/middle.png" alt="">
                <div class="play-middle">
                    <i class="fa-solid fa-play">
                        <!-- <a class="slider-middle" href="https://www.youtube.com/watch?v=JFf8I_8Ubv4"></a> -->
                    </i>
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