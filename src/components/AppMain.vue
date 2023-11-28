<script>
import AppContent from './AppContent.vue';
import AppMenu from './AppMenu.vue';


export default {
    name: "AppMain",

    components: {
        AppContent,
        AppMenu
    }

}

</script>

<template>
    <AppContent />
    <AppMenu />
</template>

<style scoped></style>
