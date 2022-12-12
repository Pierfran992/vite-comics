<script>
export default {

}
</script>

<template>
    <!-- creo la section che prende tutta la lunghezza della pagina con colozione #0282f9  -->
    <section>
        <!-- creo il container in cui inserire i vari link -->
        <div class="container">
            <div class="slot_link">
                <a href="#">
                    <div>
                        <img src="../../assets/img/buy-comics-digital-comics.png" alt="buy digital comics">
                    </div>

                    <span>DIGITAL COMICS</span>
                </a>
            </div>
            <div class="slot_link">
                <a href="#">
                    <div>
                        <img src="../../assets/imG/buy-comics-merchandise.png" alt="buy comics merchandise">
                    </div>

                    <span>DC MERCHANDISE</span>
                </a>
            </div>
            <div class="slot_link">
                <a href="#">
                    <div>
                        <img src="../../assets/img/buy-comics-subscriptions.png" alt="buy comics subscriptions">
                    </div>

                    <span>SUBSCRIPTIONS</span>
                </a>
            </div>
            <div class="slot_link">
                <a href="#">
                    <div>
                        <img src="../../assets/img/buy-comics-shop-locator.png" alt="buy comics shop locators">
                    </div>

                    <span>COMIC SHOP LOCATOR</span>
                </a>
            </div>
            <div class="slot_link">
                <a href="#">
                    <div>
                        <img src="../../assets/img/buy-dc-power-visa.svg" alt="buy dc power visa">
                    </div>

                    <span>DC POWER VISA</span>
                </a>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

section {
    background-color: #0282f9;
    color: $primaryColor;
    height: 100px;
}

.container {
    height: 100%;
    @include between();
    gap: 20px;
}

.slot_link {
    width: calc((100% - 20px) / 5);

    a {
        color: $primaryColor;
        height: 100px;
        font-size: 13px;
        text-decoration: none;
        @include center();

        div {
            height: 60px;
            margin-right: 10px;
        }
    }
}
</style>