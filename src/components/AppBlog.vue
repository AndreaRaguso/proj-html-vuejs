<script>

export default {
    name: 'AppBlog',
    data() {
        return {

        }
    },
}

</script>

<template>

    <!-- SECTION BLOG  -->
    <section id="blog">
        <!-- BLOG CONTAINER -->
        <div class=" position-relative">
            <!-- SHAPE TOP CONTAINER -->
            <div class=" position-absolute">
                <img class="w-100 img-fluid" src="../assets/img/shape-top.png" alt="shapetop">
            </div>
            <!-- COUNT CONTAINER -->
            <div class="count">
                <div class="content">
                    <!-- TEXT BLOG -->
                    <div class="text-blog">
                        <h5>We Create New Worlds!</h5>
                        <h2>Want Tips On Your Storytelling?</h2>
                        <p>Join our newsletter for tips on how to elevate your brand through storytelling</p>
                        <!-- BOX EMAILS NEWSLETTER -->
                        <div class="position-relative">
                            <input class="text-input" type="email" placeholder="Enter you email">
                            <input class="text-submit" type="submit" value="Submit">
                        </div>
                    </div>
                </div>
            </div>
            <!-- SHPAE BOTTOM CONTAINER -->
            <div class="position-absolute shape-b">
                <img class="w-100 img-fluid" src="../assets/img/shape-bottom.png" alt="shapebottom">
            </div>
        </div>

    </section>

</template>

<style lang="scss" scoped>

</style>