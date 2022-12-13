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
        <div class="container">
            <div class="badge">
                <h2>CURRENT SERIES</h2>
            </div>
            <!-- richiamo il componente che contiene le card dei fumetti -->
            <ListCard />
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

section {
    background-color: #1c1c1c;
    padding: 50px 0;
}

.badge {
    background-color: $secondaryColor;
    width: fit-content;
    font-size: 20px;
    padding: 10px 30px;
    position: relative;
    top: -80px;
}
</style>