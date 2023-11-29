<script>
export default {
    name: "AppFooterBottom",

    data() {
        return {
            Logos: [
                "footer-facebook.png", "footer-twitter.png", "footer-youtube.png", "footer-pinterest.png", "footer-periscope.png"
            ]
        }
    },
    methods: {
        getImagePath(img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <div class="wrapper">
        <div class="container p-3">
            <div class="row">
                <div class="col-6">
                    <button type="button" class="btn btn-dark mybtn">SIGN-UP NOW!</button>
                </div>
                <div class="col-6 d-flex">
                    <h4 class="textblue text-center">FOLLOW US</h4>
                    <img class="ms-2" v-for="logo in Logos" :src="getImagePath(logo)" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.wrapper {
    background-color: #303030;
}

.mybtn {
    border: solid 1px #0282F9;
}

.textblue {
    color: #0282F9;
}
</style>