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

<template lang="">
    <div class="col-4">
        <img class="img-fluid mb-3" :src="getImagePath(card.imgName)" alt="">
        <h2>{{card.title}}</h2>
        <span>{{card.price}}</span>
    </div>
</template>

<style lang="scss" scoped>
@use "../../../styles/partials/variables" as *;

img:hover {
    filter: brightness(50%);
    transition: all 1s;
}

span {
    color: $brand_tertiary;
}
</style>