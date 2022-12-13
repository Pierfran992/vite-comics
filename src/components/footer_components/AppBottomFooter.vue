<script>
export default {
    name: "AppBottomFooter"
}
</script>

<template>
    <section>
        <div class="container">
            <!-- creo il bottone per la registrazine al sito -->
            <div class="botton">
                SIGN-UP NOW!
            </div>

            <!-- creo il contenitori dei link per i social -->
            <div class="social">
                <h4>FOLLOW US</h4>

                <div class="slot_link">
                    <a href="#">
                        <img src="../../assets/img/footer-facebook.png" alt="facebook">
                    </a>
                </div>
                <div class="slot_link">
                    <a href="#">
                        <img src="../../assets/img/footer-twitter.png" alt="twitter">
                    </a>
                </div>
                <div class="slot_link">
                    <a href="#">
                        <img src="../../assets/img/footer-youtube.png" alt="youtube">
                    </a>
                </div>
                <div class="slot_link">
                    <a href="#">
                        <img src="../../assets/img/footer-pinterest.png" alt="pinterest">
                    </a>
                </div>
                <div class="slot_link">
                    <a href="#">
                        <img src="../../assets/img/footer-periscope.png" alt="periscope">
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

section {
    background-color: #303030;
    height: 100px;
}

.container {
    height: 100%;
    @include between();

    .botton {
        color: $primaryColor;
        width: fit-content;
        padding: 15px;
        border: solid 2px $secondaryColor;
    }

    .social {
        @include between();
        gap: 20px;

        h4 {
            color: $secondaryColor;
        }

        .slot_link {
            width: 40px;
            height: 40px;
        }
    }
}
</style>