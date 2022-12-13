<script>
export default {
    name: "Jumbo"
}
</script>

<template>
    <!-- creo il div che avrà come sfondo l'immagine del jumbotron -->
    <div class="jumbo"></div>
</template>

<style lang="scss" scoped>
.jumbo {
    height: 400px;
    background-image: url("../assets/img/jumbotron.jpg");
    background-size: cover;
}
</style>