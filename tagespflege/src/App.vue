<template>
    <Navbar />
    <router-view />
</template>

<script>
import Navbar from "@/components/Navbar.vue";

export default {
    name: "App",
    components: {
        Navbar,
    },
};
</script>

<style>
body {
    margin: 0;
    background-color: white;
    font-family: "Work Sans", sans-serif;
    font-weight: 400;
}
</style>
