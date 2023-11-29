<script>
export default {
    name: "AppContent",
    props: {
        comic: Object
    }
}

</script>

<template>
    <div class="col-2 bg-transparent">
        <img :src="comic.thumb" class="img-fluid cover" alt="...">
        <div class="">
            <p class="text-white">{{ comic.series }}</p>
        </div>
    </div>
</template>

<style scoped>
.cover {
    width: 10rem;
    height: 10rem;
}
</style>