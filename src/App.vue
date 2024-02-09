<script>

import HeaderNav from './components/HeaderNav.vue';
import MainSection from './components/MainSection.vue';
import CardFumetti from './components/CardFumetti.vue';
import LastMainSection from './components/LastMainSection.vue';
import FooterContact from './components/FooterContact.vue';

export default {
    components: {
        HeaderNav,
        MainSection,
        CardFumetti,
        LastMainSection,
        FooterContact
    }
}

</script>

<template>
    <HeaderNav/>
    <MainSection></MainSection>
    <CardFumetti></CardFumetti>
    <LastMainSection></LastMainSection>
    <FooterContact></FooterContact>
</template>

<style lang="scss">

</style>

<!-- <style lang="scss">
@use './SCSS/styles.scss'
</style> -->
