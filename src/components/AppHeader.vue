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
        <span class="plus">+</span>
        <div class="demos">
            <i class="fa-solid fa-desktop"></i>
            <span>Demos</span>
        </div>
        <div class="on-sale">
            <i class="fa-solid fa-desktop"></i>
            <span>On Sale</span>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

header {
    // height: 50rem;
    background-image: url(../assets/img/home-background-hero-scaled.jpg);
    background-size: cover;
    position: relative;

    span.plus {
        font-size: 2rem;
        padding: 0 1rem 0.4rem;
        border-radius: 100%;
        color: $brand_primary;
        background-color: $brand_tertiary;
        position: absolute;
        top: 1rem;
        right: 1rem;
    }

    div.demos {

        width: fit-content;
        padding: .5rem;
        background-color: $brand_primary;
        position: absolute;
        top: 10rem;
        right: 1rem;
        text-align: center;
        border-radius: 5px;

        i {
            color: $icon_color;
        }

        span {
            display: block;
            color: $text_color;
            font-size: .9rem;
            font-weight: 500;
        }

    }

    div.on-sale {

        width: fit-content;
        padding: .5rem;
        background-color: $brand_primary;
        position: absolute;
        top: 14.2rem;
        right: 1rem;
        text-align: center;
        border-radius: 5px;

        i {
            color: $icon_color;
        }

        span {
            display: block;
            color: $text_color;
            font-size: .83rem;
            font-weight: 500;
        }

    }
}
</style>