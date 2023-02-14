<script>

export default {
    name: 'AppCount',
    data() {
        return {

        }
    },
}

</script>

<template>

    <!-- SECTION COUNTER -->
    <section id="counter">
        <div class=" position-relative">
            <!-- SHAPE TOP CONTAINER -->
            <div class=" position-absolute">
                <img class="w-100 img-fluid" src="../assets/img/shape-top.png" alt="shapetop">
            </div>
            <!-- GLOBE BACKGROUND CONTAINER -->
            <div class="globe-count">
                <img class="img-fluid"  src="../assets/img/globe.png" alt="globe">
            </div>
            <!-- COUNT CONTAINER -->
            <div class="count">
                <div class="content">
                    <!-- TEXT COUNTER -->
                    <h1 class="text-center">Anidio Quick Facts</h1>
                    <!-- CARDS COUNTER -->
                    <div class="d-flex my-5">
                        <div class="card-count me-4">
                            <h1><span id="n1"></span>+</h1>
                            <h5>Projects done</h5>
                        </div>
                        <div class="card-count me-4">
                            <h1><span id="n2"></span>+</h1>
                            <h5>Happy Clients</h5>
                        </div>
                        <div class="card-count me-4">
                            <h1><span id="n3"></span>+</h1>
                            <h5>Team Members</h5>
                        </div>
                        <div class="card-count me-4">
                            <h1><span id="n4"></span>+</h1>
                            <h5>Years on the market</h5>
                        </div>
                    </div>
                </div>
            </div>
            <!-- SHAPE BOTTOM CONTAINER -->
            <div class="position-absolute shape-b">
                <img class="w-100 img-fluid" src="../assets/img/shape-bottom.png" alt="shapebottom">
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>

</style>