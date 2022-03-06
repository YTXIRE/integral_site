<template>
    <div>
        <v-parallax height='1000' src="@/assets/contacts.jpg">
            <v-row align="center" justify="center">
                <v-col class="text-center text--underline" cols="12">
                    <h1 class="display-3 font-weight-bold mb-4 ">Наши контакты</h1>
                    <h1 class="font-weight-light text-uppercase">г. Пермь, ул. Чкалова, дом 9 литера Е, офис 521</h1>
                    <h1 class="font-weight-light text-uppercase">Тел/факс. <a href="tel:83422498610">8(342)249-86-10</a>
                    </h1>
                    <h1 class="font-weight-light text-uppercase">e-mail: <a href="mailto:office@integralperm.ru">office@integralperm.ru</a>
                    </h1>
                </v-col>
            </v-row>
            <p>© Все права защищены. 2006 - {{ year }}</p>
        </v-parallax>
    </div>
</template>

<script>
export default {
    data: () => ({
        year: new Date().getFullYear()
    }),
}
</script>

<style scoped>
a {
    color: white !important;
    text-decoration: none;
}

a:hover {
    color: lawngreen !important;
    transition: all 0.5s;
}

p {
    text-align: center;
    font-size: 14px;
}
</style>