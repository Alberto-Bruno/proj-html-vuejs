<script>
import HeaderApp from './components/HeaderApp.vue';
import MainWelcome from './components/Main/MainWelcome.vue';
import MainSpecialEvents from './components/Main/MainSpecialEvents.vue';
import FooterApp from './components/FooterApp.vue';

export default {
    data() {
        return {

        }
    },
    components: {
        HeaderApp,
        MainWelcome,
        MainSpecialEvents,
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
    background-color: #161c2b;
}
</style>
