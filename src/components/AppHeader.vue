<script>
export default {
    data() {
        return {
            navItems: [
                {
                    text: "characters",
                    active: false
                },
                {
                    text: "comics",
                    active: true
                },
                {
                    text: "movies",
                    active: false
                },
                {
                    text: "tv",
                    active: false
                },
                {
                    text: "games",
                    active: false
                },
                {
                    text: "collectibles",
                    active: false
                },
                {
                    text: "videos",
                    active: false
                },
                {
                    text: "fans",
                    active: false
                },
                {
                    text: "news",
                    active: false
                },
                {
                    text: "shop",
                    active: false
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container-lg">
            <div class="row">
                <div class="col-4">
                    <a href="#">
                        <img class="p-3" src="../assets/img/dc-logo.png" alt="DC main logo">
                    </a>
                </div>
                <div class="col-8">
                    <ul>
                        <li v-for="navItem in navItems" :class="(navItem.active) ? 'active' : ''">
                            {{ navItem.text }}
                        </li>
                    </ul>
                </div>
            </div>
        </div>

    </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

header {
    background-color: white;

    img {
        width: 115px;
    }

    ul {
        display: flex;
        align-items: center;
        justify-content: end;
        margin-bottom: 0;

        li {
            font-size: 12px;
            font-weight: 700;
            margin: 0 1rem;
            padding: calc((115px/2) - 10.5px) 0;
            border-bottom: 3px solid transparent;
            text-transform: uppercase;

            &.active {
                color: $main-color;
                border-bottom: 3px solid $main-color;
            }
        }
    }
}
</style>