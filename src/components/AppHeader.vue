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
                <div>
                    <ul class="d-flex header-list align-items-center">
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
        <div class="container-lg">
            <div class="text-center jumbo-text">
                <h5>Image, Create, Experience</h5>
                <h1>We Animate</h1>
                <h1>Whit Ninja-Like Precision</h1>
                <p>We are a character-driven animation studio striving to make high-quality animations.</p>
                <div>
                    <a href="" class="button btn-back text-dark mx-4">Start a Project</a>
                    <a href="" class="button text-white">Portfolio</a>
                </div>
            </div>
        </div>
    </section>

</template>

<style lang="scss">

</style>