<script>
export default {
    name: "AppMiddleFooter"
}
</script>

<template>
    <!-- creo la sezione principale che prenderà l'intera lunghezza della pagina -->
    <section>
        <div class="container">
            <!-- slot che conterrà i vari menu del footer -->
            <div class="container_menu">

            </div>

            <!-- slot che conterrà il logo del footer -->
            <div class="slot_big_logo">
                <img src="../../assets/img/dc-logo-bg.png" alt="big logo">
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

section {
    background-image: url("../../assets/img/footer-bg.jpg");
    background-size: cover;
    height: 400px;
    overflow: hidden;
}

.container {
    height: 100%;
    @include between();
}
</style>