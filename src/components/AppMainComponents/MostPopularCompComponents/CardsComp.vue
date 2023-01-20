<script>
import CardComp from "./CardComp.vue"

export default {
    components: {
        CardComp,
    },
    data() {
        return {
            mostPopularProductsCards: [
                {
                    imgName: "skin-on-fries-400x571",
                    title: "Skin On Fries",
                    price: "$3.00-$6.00"
                },
                {
                    imgName: "choco-cookie-frappe-400x571",
                    title: "Choco Cookie Frappe",
                    price: "$4.99"
                },
                {
                    imgName: "donut-burger-400x571",
                    title: "The Donut Burger",
                    price: "$6.99"
                },
            ]
        }
    },
}
</script>

<template>
    <div class="row text-center">
        <CardComp v-for="singleCard in mostPopularProductsCards" :card="singleCard" />
        <div class="col">
            <a class="btn rounded-pill">START YOUR ORDER
                <i class="fa-solid fa-circle-arrow-right"></i>
            </a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../../../styles/partials/variables" as *;

a {
    background-color: $brand_tertiary;
    padding: .5rem 1.5rem;
    font-weight: 500;
    color: $brand_primary;
    margin-top: 4rem;
    margin-bottom: 10rem;

    i {
        margin-left: .7rem;
    }
}
</style>