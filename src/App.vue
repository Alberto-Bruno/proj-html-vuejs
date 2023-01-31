<script>
import HeaderApp from './components/HeaderApp.vue';
import MainSpecialEvents from './components/Main/MainSpecialEvents.vue';
import MainWelcome from './components/Main/MainWelcome.vue';
import FooterApp from './components/FooterApp.vue';

export default {
    data() {
        return {

        }
    },
    components: {
        HeaderApp,
        MainSpecialEvents,
        MainWelcome,
        FooterApp
    }
}
</script>

<template>
    <HeaderApp></HeaderApp>
    <MainWelcome></MainWelcome>
    <MainSpecialEvents></MainSpecialEvents>
    <FooterApp></FooterApp>
</template>

<style scoped lang="scss">
@use './assets/Styles/style.scss' as*;

* {
    background-color: #1b1e26;
}
</style>
