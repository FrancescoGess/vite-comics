<script>

import HeaderNav from './components/HeaderNav.vue';
import MainSection from './components/MainSection.vue';
import CardFumetti from './components/CardFumetti.vue';
import LastMainSection from './components/LastMainSection.vue';
import FooterContact from './components/FooterContact.vue';
import Jumbotron from './components/Jumbotron.vue';

export default {
    components: {
        HeaderNav,
        Jumbotron,
        CardFumetti,
        MainSection,
        LastMainSection,
        FooterContact
    }
}

</script>

<template>
    <HeaderNav/>
    <Jumbotron></Jumbotron>
    <CardFumetti></CardFumetti>
    <MainSection></MainSection>
    <LastMainSection></LastMainSection>
    <FooterContact></FooterContact>
</template>

<style lang="scss">

</style>

<!-- <style lang="scss">
@use './SCSS/styles.scss'
</style> -->
