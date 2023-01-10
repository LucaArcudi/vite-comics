<template>
    <header>
        <div class="container-lg">
            <div class="row">
                <div class="col-4">
                    <a href="#">
                        <img class="p-3" src="../assets/img/dc-logo.png" alt="DC main logo">
                    </a>
                </div>
                <div class="col-8 d-flex align-items-center justify-content-center">
                    <ul class="d-flex">
                        <li v-for="navItem in navItems" :class="(navItem.active) ? 'active' : ''">
                            {{ navItem.text.toUpperCase() }}
                        </li>
                    </ul>
                </div>
            </div>
        </div>

    </header>
</template>

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

<style lang="scss">
header {
    background-color: white;
    margin-top: 2vh;

    img {
        width: 115px;
    }

    ul {
        list-style-type: none;
        margin-bottom: 0;

        li {
            font-size: 12px;
            font-weight: 700;
            padding: 0 1rem;

            &:hover {
                color: #0282F9;
            }
        }
    }
}


.active {
    color: #0282F9;
}
</style>