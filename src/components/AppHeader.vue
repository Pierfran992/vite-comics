<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false,
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true,
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false,
                },
                {
                    text: "TV",
                    url: "#",
                    current: false,
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false,
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false,
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false,
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false,
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false,
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false,
                },
            ],
        }
    },
}
</script>

<template>
    <header>
        <div class="container">
            <!-- slot contenente il logo -->
            <div class="slot_logo">
                <a href="#">
                    <img src="../assets/img/dc-logo.png" alt="logo_DC">
                </a>
            </div>

            <!-- menu di navigazione -->
            <div class="slot_nav_menu">
                <ul>
                    <li v-for="(link, index) in links" :key="index">
                        <a :class="{ active: link.current }" :href="link.url">{{ link.text }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

header {
    height: 100px;
}

.container {
    height: 100%;
    @include between();
}

.slot_logo {
    width: 100px;
    height: 80px;
}

.slot_nav_menu {
    height: 100%;

    ul {
        @include center();
        height: 100%;

        li {
            list-style-type: none;
            margin-left: 20px;

            a {
                text-decoration: none;
                font-size: 13px;
                font-weight: 500;
                height: 100px;
                line-height: 100px;
                display: inline-block;

                &.active,
                &:hover {
                    color: #0282f9;
                    border-bottom: solid 3px #0282f9;
                }

            }
        }
    }
}
</style>
