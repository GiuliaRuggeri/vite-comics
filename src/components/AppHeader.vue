<script>
export default {
    name: "AppHeader",

    data() {
        return {
            Links: [
                {
                    text: "Characters",
                    url: "#characters",
                },
                {
                    text: "Comics",
                    url: "#comics",
                },
                {
                    text: "Movies",
                    url: "#movies",
                },
                {
                    text: "TV",
                    url: "#tv",
                },
                {
                    text: "Games",
                    url: "#games",
                },
                {
                    text: "Collectibles",
                    url: "#collectibles",
                },
                {
                    text: "Videos",
                    url: "#videos",
                },
                {
                    text: "Fans",
                    url: "#fans",
                },
                {
                    text: "News",
                    url: "#news",
                },
                {
                    text: "Shop",
                    url: "#shop",
                }
            ]
        }
    },
}



</script>

<template>
    <nav class="navbar p-0">
        <div class="container">
            <img src="../assets/img/dc-logo.png" class="navbar-brand logo">
            <form class="d-flex" role="search">
                <ul class="navbar-nav d-flex flex-row">
                    <li class="nav-item ms-2 link" v-for="link in Links">
                        <a class=" nav-link active " aria-current="page" :href="link.url">{{ link.text }}</a>
                    </li>

                </ul>
            </form>
        </div>
    </nav>
</template>

<style scoped>
.logo {
    width: 4rem;
}

li {
    border-bottom: solid 2px transparent;
    line-height: 4em;

}

.link:hover {
    border-bottom: solid 3px #0282F9;
}

.link:hover>a {
    color: #0282F9
}
</style>
