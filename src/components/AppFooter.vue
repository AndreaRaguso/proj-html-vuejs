<script>

export default {
    name: 'AppFooter',
    data() {
        return {

        }
    },
}

</script>

<template>
    <!-- FOOTER  -->
    <footer>
        <!-- FOOTER CONTAINER -->
        <div class="container-lg">
            <div class="d-flex justify-content-between align-items-center">
                <!-- LOGO FOOTER -->
                <div>
                    <img src="../assets/img/footer-logo.png" alt="logo-f">
                </div>
                <!-- NAV FOOTER -->
                <nav>
                    <ul class="d-flex">
                        <li>
                            <a href="">About Us</a>
                        </li>
                        <li>
                            <a href="">Portfolio</a>
                        </li>
                        <li>
                            <a href="">Pricing</a>
                        </li>
                        <li>
                            <a href="">Career</a>
                        </li>
                        <li>
                            <a href="">Contact</a>
                        </li>
                    </ul>
                </nav>
            </div>
            <!-- HORIZONTAL RULE FOOTER -->
            <hr>
            <div class="d-flex justify-content-between">
                <!-- CREDITS FOOTER -->
                <div>
                    <em>Copyright&#64 2022 <span class="softvirus">Softvirus</span>. All rights reserved.</em>
                </div>
                <!-- SOCIALS FOOTERS -->
                <div>
                    <div class="socials d-flex justify-content-center mb-3">
                        <a href="#"><i class="fab fa-facebook-square fa-2x logo me-3"></i></a>
                        <a href="#"><i class="fab fa-twitter fa-2x logo me-3"></i></a>
                        <a href="#"><i class="fab fa-instagram fa-2x logo"></i></a>
                    </div>
                </div>
            </div>
        </div>
    </footer>


</template>

<style lang="scss" scoped>

</style>