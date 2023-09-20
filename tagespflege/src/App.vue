<template>
    <Navbar />
    <router-view />
    <div class="footer">
        <div class="kontakt">
            <ul>
                Adresse<!--Adresse und Kontaktdaten sowie Name-->
            </ul>
        </div>
        <div class="quicklinks">
            <ul>
                <li>links</li><!--Navbar quicklinks-->
            </ul>
        </div>
        <div class="footprint">
            <p>
                Autor<!--Autor und publishing Lizenz-->
            </p>
        </div>
    </div>
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
