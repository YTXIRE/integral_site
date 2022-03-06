<template>
    <div>
        <v-parallax height='1000' src="@/assets/gallery.jpg">
            <v-row align="center" justify="center">
                <v-col class="text-center text--underline" cols="11">
                    <h1>ЧЕМ МЫ ЗАНИМАЕМСЯ</h1>
                    <gallery :images="images" :index="index" @close="index = null"></gallery>
                    <div
                            v-for="(image, imageIndex) in images"
                            :key="imageIndex"
                            :style="{backgroundImage: 'url(' + image + ')', width: '390px', height: '200px'}"
                            class="image"
                            @click="index = imageIndex"
                    />

                </v-col>
            </v-row>
        </v-parallax>
    </div>
</template>
<script>
import VueGallery from 'vue-gallery';

export default {
    data: function () {
        return {
            images: [
                'https://i.ibb.co/6sFJ5bz/01.jpg',
                'https://i.ibb.co/py26L6v/02.jpg',
                'https://i.ibb.co/QMQT0SY/03.jpg',
                'https://i.ibb.co/zV8hxGW/04.jpg',
                'https://i.ibb.co/NS82m9x/05.jpg',
                'https://i.ibb.co/WWfV2FK/06.jpg',
                'https://i.ibb.co/JpL70nr/07.jpg',
                'https://i.ibb.co/3kWvwmf/08.jpg',
            ],
            index: null
        };
    },

    components: {
        'gallery': VueGallery
    },
}
</script>

<style scoped>
.image {
    float: left;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
    border: 1px solid #ebebeb;
    margin: 20px;
}
</style>