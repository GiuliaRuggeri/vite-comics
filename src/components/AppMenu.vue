<script>

export default {
    name: "AppMenu",

    data() {
        return {
            Items: [
                {
                    img: "buy-comics-digital-comics.png",
                    description: "DIGITAL COMICS",
                },
                {
                    img: "buy-comics-merchandise.png",
                    description: "DC MERCHANDISE",
                },

                {
                    img: "buy-comics-subscriptions.png",
                    description: "SUBSCRIPTION",
                },
                {
                    img: "buy-comics-shop-locator.png",
                    description: "COMIC SHOP LOCATOR",
                },
                {
                    img: "buy-dc-power-visa.svg",
                    description: "DC POWER VISA",
                }
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
    <div class="bg-blue">
        <div class="container menuwrapper">
            <div v-for="item in Items">
                <img :src="getImagePath(item.img)" alt="" class="images">
                <span class="ms-1 text-white">{{ item.description }}</span>

            </div>

        </div>


    </div>
</template>

<style scoped>
.menuwrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 2rem;
}

.images {
    width: 2rem;
}

.bg-blue {
    background-color: #0282F9;
}
</style>