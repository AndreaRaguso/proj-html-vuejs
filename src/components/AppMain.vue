<script>

import AppSmart from '../components/AppSmart.vue';
import AppCount from '../components/AppCount.vue';
import AppWorks from '../components/AppWorks.vue';
import AppProcess from '../components/AppProcess.vue';
import AppTeam from '../components/AppTeam.vue';

export default {
    name: 'AppMain',
    components: {
        AppSmart,
        AppCount,
        AppWorks,
        AppProcess,
        AppTeam,
    },
    data() {
        return {

        }
    },
}

</script>

<template>

    <AppSmart />
    <AppCount />
    <AppWorks />
    <AppProcess />
    <AppTeam />

</template>

<style lang="scss" scoped>

</style>