<script>
export default {

}
</script>

<template >
    <section class="footer-bot container-lg">
        <div class="row text-center">
            <div class="col">
                <img src="../../assets/img/takeout-logo.png" alt="">
                <h2>
                    Stay In The Loop
                </h2>

                <p>
                    Sign up to receive up to date news and offers directly in your inbox:
                </p>

                <form>
                    <input type="text" placeholder="you@email.com"><br>
                    <a class="btn rounded-pill">VIEW OUR MENU
                        <i class="fa-solid fa-circle-arrow-right"></i>
                    </a>
                </form>
                <div class="icons">
                    <i class="fa-brands fa-facebook-f"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-instagram"></i>
                    <i class="fa-brands fa-linkedin-in"></i>
                    <i class="fa-solid fa-rss"></i>
                    <i class="fa-brands fa-youtube"></i>
                    <i class="fa-regular fa-envelope"></i>
                </div>


                <p class="credits">
                    &#169; Copyright 2012 - 2020 | Avada Theme by
                    <span>ThemeFusion</span>
                    | All Rights Reserved | Powered by
                    <span>WordPress</span>
                </p>


            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;

.row {
    padding-top: 5rem;
    padding-bottom: 10rem;

    p {
        color: $brand_primary;
        font-weight: 500;
    }

    h2 {
        font-size: 3rem;
        font-weight: 500;
        color: $brand_secondary;
        margin-bottom: 1rem;

    }

    input {
        margin-bottom: 1rem;
        padding: .5rem 1rem;
        width: 60%;
        border-radius: 10rem;
    }

    a {
        background-color: $brand_tertiary;
        padding: .5rem 1.5rem;
        font-weight: 500;
        color: $brand_primary;
        width: 60%;
        margin-bottom: 2rem;

        i {
            margin-left: .7rem;
        }
    }

    i {
        margin: 0 1rem;
        color: $brand_primary;
    }

    div.icons {
        margin-bottom: 1rem;
    }

    p.credits {
        font-size: .7rem;
        color: $brand_secondary;

        span {
            color: $brand_primary;
        }
    }

}
</style>