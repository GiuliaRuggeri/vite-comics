<script>

export default {
    name: "AppMenu",

    data() {
        return {
            Items: [
                {
                    img: "../src/assets/img/buy-comics-digital-comics.png",
                    description: "DIGITAL COMICS",
                },
                {
                    img: "../src/assets/img/buy-comics-merchandise.png",
                    description: "DC MERCHANDISE",
                },

                {
                    img: "../src/assets/img/buy-comics-subscriptions.png",
                    description: "SUBSCRIPTION",
                },
                {
                    img: "../src/assets/img/buy-comics-shop-locator.png",
                    description: "COMIC SHOP LOCATOR",
                },
                {
                    img: "../src/assets/img/buy-dc-power-visa.svg",
                    description: "DC POWER VISA",
                }
            ]
        }
    },
}

</script>

<template>
    <div class="bg-blue">
        <div class="container menuwrapper">
            <div v-for="item in Items">
                <img :src="item.img" alt="" class="images image-fluid">
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
    width: 3rem;
}

.bg-blue {
    background-color: #0282F9;
}
</style>