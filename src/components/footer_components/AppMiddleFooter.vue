<script>
export default {
    name: "AppMiddleFooter",
    data() {
        return {
            menu: [
                {
                    title: "DC COMICS",
                    link: [
                        {
                            url: "#",
                            text: "Characters"
                        },
                        {
                            url: "#",
                            text: "Comics"
                        },
                        {
                            url: "#",
                            text: "Movies"
                        },
                        {
                            url: "#",
                            text: "TV"
                        },
                        {
                            url: "#",
                            text: "Games"
                        },
                        {
                            url: "#",
                            text: "Videos"
                        },
                        {
                            url: "#",
                            text: "News"
                        },
                    ]
                },
                {
                    title: "SHOP",
                    link: [
                        {
                            url: "#",
                            text: "Shop DC"
                        },
                        {
                            url: "#",
                            text: "Shop DC Collectibles"
                        },
                    ]
                },
                {
                    title: "DC",
                    link: [
                        {
                            url: "#",
                            text: "Terms Of Use"
                        },
                        {
                            url: "#",
                            text: "Privacy policy (New)"
                        },
                        {
                            url: "#",
                            text: "Ad Choices"
                        },
                        {
                            url: "#",
                            text: "Advertising"
                        },
                        {
                            url: "#",
                            text: "Jobs"
                        },
                        {
                            url: "#",
                            text: "Subscriptions"
                        },
                        {
                            url: "#",
                            text: "Talent Workshops"
                        },
                        {
                            url: "#",
                            text: "CPSC Certificates"
                        },
                        {
                            url: "#",
                            text: "Ratings"
                        },
                        {
                            url: "#",
                            text: "Shop Help"
                        },
                        {
                            url: "#",
                            text: "Contact Us"
                        },
                    ]
                },
                {
                    title: "SITES",
                    link: [
                        {
                            url: "#",
                            text: "DC"
                        },
                        {
                            url: "#",
                            text: "MAD Magazine"
                        },
                        {
                            url: "#",
                            text: "DC kids"
                        },
                        {
                            url: "#",
                            text: "DC Universe"
                        },
                        {
                            url: "#",
                            text: "DC Power Visa"
                        },
                    ]
                }
            ]
        }
    }
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