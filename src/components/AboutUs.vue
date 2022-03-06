<template>
    <div>
        <v-parallax class="opacity" height='1000'>
            <v-row align="center" justify="center">
                <v-col class="text-center text--underline" cols="12">
                    <h1 class="display-4 font-weight-bold mb-4 ">О нас</h1>
                    <h1 class="font-weight-light text-uppercase">Наша компания основана в 2006 году.
                        Мы работаем в сфере оптовых поставок песка, щебня, арматуры и прочих стоительных материалов.
                        За время нашей работы мы зарекомендовали себя надежными партнерами, готовыми к
                        сотрудничеству.</h1>
                </v-col>
            </v-row>
        </v-parallax>
    </div>
</template>

<style scoped>
.opacity {
    position: relative;
    color: #fff;
    text-shadow: 0 0 0.5px rgba(255, 255, 255, 0.25);
    text-align: center;
    background: #35b88f url("../assets/banner.svg") bottom center no-repeat;
    padding: 5em 0 5em 0;
    margin: 0;
    background-size: 125% auto;
}
</style>