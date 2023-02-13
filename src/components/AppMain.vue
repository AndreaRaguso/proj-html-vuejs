<script>

import AppSmart from '../components/AppSmart.vue';
import AppCount from '../components/AppCount.vue';
import AppWorks from '../components/AppWorks.vue';

export default {
    name: 'AppMain',
    components: {
        AppSmart,
        AppCount,
        AppWorks
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

</template>

<style lang="scss" scoped>

</style>