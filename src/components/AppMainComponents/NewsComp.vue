<script>
import NewsCardsComp from './NewsComponents/NewsCardsComp.vue';

export default {
    components: {
        NewsCardsComp,
    }
}
</script>

<template>
    <section class="news">
        <div class="wrapper container-lg">
            <div class="row justify-content-between">
                <div class="col-6">
                    <h1>Latest News</h1>
                </div>
                <div class="col-3">
                    <a class="btn rounded-pill">READ MORE NEWS
                        <i class="fa-solid fa-circle-arrow-right"></i>
                    </a>
                </div>
            </div>
            <NewsCardsComp />
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
</style>