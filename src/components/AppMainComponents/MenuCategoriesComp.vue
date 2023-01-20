<script>
import MenuCategoriesCardsComp from './MenuCategoriesComponents/MenuCategoriesCardsComp.vue';

export default {
    components: {
        MenuCategoriesCardsComp,
    }
}
</script>

<template>
    <section class="menu-categories">
        <div class="wrapper container-lg">
            <div class="row justify-content-between">
                <div class="col-6">
                    <h1>Menu Categories</h1>
                </div>
                <div class="col-3">
                    <a class="btn rounded-pill">VIEW THE FULL MENU
                        <i class="fa-solid fa-circle-arrow-right"></i>
                    </a>
                </div>
            </div>
            <MenuCategoriesCardsComp />
            <div class="row intolerant-food">
                <div class="col-3">
                    <i class="fa-solid fa-leaf"></i>
                    <h4>Vegetarin</h4>
                </div>
                <div class="col-3">
                    <i class="fa-solid fa-wheat-awn"></i>
                    <h4>Gluten Free</h4>
                </div>
                <div class="col-3">
                    <i class="fa-solid fa-bottle-droplet"></i>
                    <h4>Dairy Free</h4>
                </div>
                <div class="col-3">
                    <i class="fa-solid fa-burger"></i>
                    <h4>Keto Friendly</h4>
                </div>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;

div.row {
    margin-bottom: 5rem;

    h1 {
        padding-top: 1rem;
    }

    a {
        background-color: $brand_tertiary;
        padding: .5rem 1.5rem;
        font-weight: 500;
        color: $brand_primary;

        i {
            margin-left: .7rem;
        }
    }
}

div.intolerant-food {
    text-align: center;
    margin-bottom: 10rem;

    i {
        font-size: 3rem;

        &.fa-leaf {
            color: $price_color;
        }

        &.fa-wheat-awn {
            color: $brand_secondary;
        }

        &.fa-bottle-droplet {
            color: #006194;
        }

        &.fa-burger {
            color: #a16d2e;
        }
    }

}
</style>