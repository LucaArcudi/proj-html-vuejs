<script>
import NewsCardComp from "./NewsCardComp.vue"

export default {
    components: {
        NewsCardComp,
    },
    data() {
        return {
            mostPopularProductsCards: [
                {
                    imgName: "pancake-burger",
                    title: "NEW: The Pancake Burger",
                    content: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quaerat rerum iusto eius corrupti provident doloribus minima quo aliquid facere, voluptatum, ipsum modi perspiciatis architecto magnam ab amet facilis, dignissimos ipsam."
                },
                {
                    imgName: "new-milkshake-menu",
                    title: "New Milkshake Menu",
                    content: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quaerat rerum iusto eius corrupti provident doloribus minima quo aliquid facere, voluptatum, ipsum modi perspiciatis architecto magnam ab amet facilis, dignissimos ipsam."
                }
            ]
        }
    },
}
</script>

<template>
    <div class="row text-center">
        <NewsCardComp v-for="singleCard in mostPopularProductsCards" :card="singleCard" />
    </div>
</template>

<style lang="scss" scoped>
@use "../../../styles/partials/variables" as *;

div.row {
    margin-bottom: 10rem;
}
</style>