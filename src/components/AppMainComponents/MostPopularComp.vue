<script>
import CardsComp from "./MostPopularCompComponents/CardsComp.vue"

export default {
    components: {
        CardsComp,
    }
}
</script>

<template>
    <section class="most-popular">
        <div class="wrapper container-lg">
            <div class="row absolute-row">
                <div class="col-2">
                    <i class="fa-regular fa-clock"></i>
                    <p>24/7 DELIVERY</p>
                </div>
                <div class="col-2">
                    <i class="fa-solid fa-burger"></i>
                    <p>OVER 100 DISHES</p>
                </div>
                <div class="col-2">
                    <i class="fa-solid fa-mobile-screen-button"></i>
                    <p>IN APP ORDERING</p>
                </div>
                <div class="col-2">
                    <i class="fa-solid fa-car"></i>
                    <p>FAST DELIVERY</p>
                </div>
            </div>
            <div class="row most-popular-title text-center">
                <div class="col">
                    <h1>Our Most Popular Dishes</h1>
                </div>
            </div>
            <CardsComp />
        </div>

        <div class="background container-fluid p-0">
            <img class="a" src="../../assets/img/svg-0.svg" alt="">
            <img class="b" src="../../assets/img/svg-0.svg" alt="">
            <img class="c" src="../../assets/img/svg-0.svg" alt="">
            <img class="d" src="../../assets/img/svg-0.svg" alt="">
        </div>
    </section>
</template>


<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;

section.most-popular {
    background-color: $brand_primary;

    .wrapper {
        background-color: $brand_primary;
        position: relative;

        .row.absolute-row {
            padding: 3rem 2rem;
            position: absolute;
            top: -2.5rem;
            width: 100%;
            background-color: $brand_primary;
            text-align: center;
            justify-content: space-between;

            i {
                margin-right: 1rem;
            }

            p {
                color: $text_color;
                display: inline;
            }
        }

        .row.most-popular-title {
            padding-top: 10rem;
            margin-bottom: 5rem;

            h1 {
                font-weight: 700;
                font-size: 3rem;
            }
        }
    }

    .background {
        background-image: url("../../assets/img/first-order-background-scaled.jpg");
        background-size: cover;
        height: 33rem;




        img.a {
            filter: opacity(.2);
        }

        img.b {
            filter: opacity(.4);
            transform: rotate(1deg) translate(-1.1rem, -27rem);
        }

        img.c {
            filter: opacity(.6);
            transform: translate(0rem, -55rem);
        }

        img.d {
            transform: translate(0rem, -83rem);
        }
    }


}
</style>