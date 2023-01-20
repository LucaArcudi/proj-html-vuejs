<script>
import MenuCategoriesCardComp from "./MenuCategoriesCardComp.vue"

export default {
    components: {
        MenuCategoriesCardComp,
    },
    data() {
        return {
            mostPopularProductsCards: [
                {
                    imgName: "appetizers-menu-background",
                    title: "Appetizers",
                },
                {
                    imgName: "burgers-menu-background",
                    title: "Burgers",
                },
                {
                    imgName: "pizza-menu-background",
                    title: "Pizzas",
                },
                {
                    imgName: "fries-menu-background",
                    title: "Fries",
                },
                {
                    imgName: "sides-menu-background",
                    title: "Sides",
                },
                {
                    imgName: "desserts-menu-background",
                    title: "Desserts",
                },
                {
                    imgName: "beverages-menu-background",
                    title: "Beverages",
                },
                {
                    imgName: "specials-menu-background",
                    title: "Specials",
                },
            ]
        }
    },
}
</script>

<template>
    <div class="row text-center">
        <MenuCategoriesCardComp v-for="singleCard in mostPopularProductsCards" :card="singleCard" />
    </div>
</template>

<style lang="scss" scoped>
@use "../../../styles/partials/variables" as *;
</style>