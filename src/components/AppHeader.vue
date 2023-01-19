<script>
import NavComp from "./AppHeaderComponents/NavComp.vue";
import MainComp from "./AppHeaderComponents/MainComp.vue";

export default {
    components: {
        NavComp,
        MainComp,
    }
}
</script>

<template>
    <header>
        <NavComp />
        <MainComp />
    </header>
</template>

<style lang="scss" scoped>
header {
    height: 50rem;
    background-image: url(../assets/img/home-background-hero-scaled.jpg);
    background-size: cover;
}
</style>