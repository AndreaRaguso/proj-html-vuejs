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

    <section id="counter">
        <div class=" position-relative">
            <div class=" position-absolute">
                <img class="w-100" src="../assets/img/shape-top.png" alt="shapetop">
            </div>
            <div class="count">
                <div class="content">
                    <h1 class="text-center">Anidio Quick Facts</h1>
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
            <div class="position-absolute shape-b">
                <img class="w-100" src="../assets/img/shape-bottom.png" alt="shapebottom">
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>

</style>