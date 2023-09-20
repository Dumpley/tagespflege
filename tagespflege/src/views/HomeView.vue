<template>
    <div class="home">
        <div class="startseite">
            <div class="intro">
                <h1>headline</h1>
                <p>description</p>
                <div class="dicover_button">
                    Erkunde
                </div>
            </div>
            <div class="startseite_bild">
                startseite Bild <!--Bild-->
            </div>
        </div>
        <div class="startseite_willkommen">
            <div class="willkommens_bild">
                Bild willkommen
            </div>
            <p>Wilkommenstext</p>
        </div>
        <div class="startseite_streckbrief">
            <ul>
                <li>Mutter Steckrief</li><!--Stechbrief über Mutter mit kleiner Beschreibung-->
            </ul>
            <div class="steckbrief_bild">
                Bild von Mutter<!-- Ein Bild von Mutter-->
            </div>
            <ul>
                <li>
                    Weiterer Steckbrief
                </li><!-- Weitere Beschreibung-->
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: "HomeView",
};
</script>

<style>
    .introductory_text {
        text-align: left;
        padding-right: 50%;
        display: block;
    }
    .title {
        background-color: aliceblue;
    }
    .descriptive_text {
        background-color: blanchedalmond;
        font-size: large;
    }
</style>
