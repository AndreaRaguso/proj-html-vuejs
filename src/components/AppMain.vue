<script>

import AppSmart from '../components/AppSmart.vue';
import AppCount from '../components/AppCount.vue';
import AppWorks from '../components/AppWorks.vue';
import AppProcess from '../components/AppProcess.vue';
import AppTeam from '../components/AppTeam.vue';
import AppWhy from '../components/AppWhy.vue';
import AppBlog from '../components/AppBlog.vue';
import BackToTop from 'vue-backtotop'

export default {
    name: 'AppMain',
    components: {
        AppSmart,
        AppCount,
        AppWorks,
        AppProcess,
        AppTeam,
        AppWhy,
        AppBlog,
        BackToTop,
    },
    data() {
        return {


        }
    },
    methods: {

    }
}

</script>

<template>

    <back-to-top bottom="50px" right="50px">
        <button type="button" class="btn btn-info btn-to-top"><i class="fa fa-chevron-up"></i></button>
    </back-to-top>
    <AppSmart />
    <AppCount />
    <AppWorks />
    <AppProcess />
    <AppTeam />
    <AppWhy />
    <AppBlog />

</template>

<style lang="scss" scoped>

</style>