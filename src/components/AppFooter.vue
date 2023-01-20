<script>
import FooterTopComponent from './AppFooterComponents/FooterTopComponent.vue';
import FooterBotComponent from './AppFooterComponents/FooterBotComponent.vue';

export default {
    components: {
        FooterTopComponent,
        FooterBotComponent
    }
}
</script>

<template>
    <footer>
        <FooterTopComponent />
        <FooterBotComponent />
    </footer>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

footer {
    background-image: url(../assets/img/footer-background-scaled.jpg);
    background-size: cover;
    position: relative;
}
</style>