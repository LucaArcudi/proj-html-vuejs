<script>
export default {
    props: {
        card: Object,
    },

    methods: {
        getImagePath: function (imgPath) {
            return new URL(`../../../assets/img/${imgPath}.jpg`, import.meta.url).href;
        },
    },
}
</script>

<template>
    <div class="col-3">
        <img class="img-fluid mb-3" :src="getImagePath(card.imgName)" alt="">
        <h4>{{ card.title }}</h4>
    </div>
</template>

<style lang="scss" scoped>
@use "../../../styles/partials/variables" as *;

div.col-3 {
    position: relative;

    img:hover {
        filter: brightness(50%);
        transition: all 1s;
    }

    h4 {
        color: $brand_primary;
        margin-bottom: 0;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translateY(-50%) translateX(-50%);
        text-transform: uppercase;
        font-weight: 700;
    }

}
</style>