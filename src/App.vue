<template>
    <v-app>
        <Header/>
        <Main />
    </v-app>
</template>

<script>
    import Header from './components/Header';
    import Main from "./components/Main";

    export default {
        name: 'App',

        components: {
            Main,
            Header,
        },
    };
</script>

<style>
    ::-webkit-scrollbar {
        width: 0;
    }

    body {
        scroll-behavior: smooth;
    }
</style>