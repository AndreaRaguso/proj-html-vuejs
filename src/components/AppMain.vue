<script>

import AppSmart from '../components/AppSmart.vue';
import AppCount from '../components/AppCount.vue';
import AppWorks from '../components/AppWorks.vue';
import AppProcess from '../components/AppProcess.vue';

export default {
    name: 'AppMain',
    components: {
        AppSmart,
        AppCount,
        AppWorks,
        AppProcess,
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

</template>

<style lang="scss" scoped>

</style>