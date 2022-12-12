<script>
import AppTopFooter from './footer_components/AppTopFooter.vue';
import AppMiddleFooter from './footer_components/AppMiddleFooter.vue';
import AppBottomFooter from './footer_components/AppBottomFooter.vue';

export default {
    name: "AppFooter",
    components: {
        AppTopFooter,
        AppMiddleFooter,
        AppBottomFooter
    }
}
</script>

<template>
    <AppTopFooter />
    <AppMiddleFooter />
    <AppBottomFooter />
</template>

<style lang="scss" scoped>

</style>