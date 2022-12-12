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
                <div class="slot_menu">
                    <h4>DC COMICS</h4>

                    <ul>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                    </ul>
                </div>
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

.container_menu {
    height: 350px;
    padding: 10px;
    @include column();
    gap: 20px;

    h4 {
        margin-bottom: 10px;
    }

    li {
        list-style: none;
    }

    a {
        color: #797979;
        text-decoration: none;
        font-size: 12px;
    }
}
</style>