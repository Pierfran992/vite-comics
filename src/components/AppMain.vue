<script>
import ListCard from './main_components/ListCard.vue';
export default {
    name: "AppMain",
    components: {
        ListCard
    }
}
</script>

<template>
    <section>
        <!-- richiamo il componente che contiene le card dei fumetti -->
        <ListCard />
    </section>
</template>

<style lang="scss" scoped>
section {
    background-color: #1c1c1c;
    padding: 50px 0;
}
</style>