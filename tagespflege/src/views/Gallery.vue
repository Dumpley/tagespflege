<template>
    <div class="gallery">
        <div class="heading">
            <h3>Photo <span>Galerie</span></h3>
        </div>
        <div class="box">
            <div class="dream">
                <img src="@/assets/test_pictures/1.jpg" />
                <img src="@/assets/test_pictures/2.jpg" />
                <div v-if="button_clicked">
                    <img src="@/assets/test_pictures/3.jpg" />
                    <img src="@/assets/test_pictures/4.jpg" />
                    <img src="@/assets/test_pictures/5.jpg" />
                </div>
            </div>
            <div class="dream">
                <img src="@/assets/test_pictures/6.jpg" />
                <img src="@/assets/test_pictures/7.jpg" />
                <div v-if="button_clicked">
                    <img src="@/assets/test_pictures/8.jpg" />
                    <img src="@/assets/test_pictures/9.jpg" />
                    <img src="@/assets/test_pictures/10.jpg" />
                </div>
            </div>
            <div class="dream">
                <img src="@/assets/test_pictures/11.jpg" />
                <img src="@/assets/test_pictures/12.jpg" />
                <div v-if="button_clicked">
                    <img src="@/assets/test_pictures/13.jpg" />
                    <img src="@/assets/test_pictures/14.jpg" />
                    <img src="@/assets/test_pictures/15.jpg" />
                </div>
            </div>
        </div>
        <div v-if="!button_clicked" @click="changeButtonTo(true)" class="btn">More</div>
    </div>
</template>

<script>
import { ref } from "vue";

export default {
    name: "Galery",
    setup() {
        const button_clicked = ref(false);

        /**
         * Takes as input a boolean for showing or not showing the rest of the pictures:
         */
        function changeButtonTo(click) {
            button_clicked.value = click;
        }

        return {
            button_clicked,
            changeButtonTo,
        };
    },
};
</script>

<style scoped>
.gallery {
    box-sizing: border-box;
    margin: 40px 20px 0px 20px;
    padding: 0;
    font-family: "Poppins", sans-serif;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.gallery .heading {
    width: 50%;
}
.gallery .heading h3 {
    font-size: 3em;
    font-weight: bolder;
    border-bottom: 3px solid #222;
    padding-bottom: 25px;
}
.gallery .heading h3 span {
    font-weight: 100;
}

.gallery .box {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}
.gallery .box .dream {
    display: flex;
    flex-direction: column;
    width: 32.5%;
}
.gallery .box .dream img {
    width: 100%;
    margin: 5px;
    border-radius: 10px;
}
.gallery .btn {
    margin: 40px 0px 70px 0px;
    background: #222;
    padding: 15px 40px;
    border-radius: 10px;
    color: white;
    font-size: 1.2em;
    font-weight: bolder;
    text-decoration: none;
    cursor: pointer;
}
@media only screen and (max-width: 670px) {
    .gallery .box {
        flex-direction: column;
    }
    .gallery .box .dream {
        width: 100%;
    }
    .gallery .heading {
        width: 100%;
    }
    .gallery .heading h3 {
        font-size: 1em;
    }
}
</style>
