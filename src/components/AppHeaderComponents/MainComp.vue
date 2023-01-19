<script>
export default {

}
</script>

<template >
    <section class="main-section container-lg">
        <div class="row">
            <div class="col">
                <p>Hungry?</p>
                <h1>
                    <span>Great Food</span> <br>
                    Delivered
                </h1>
                <a class="btn btn-danger rounded-pill">VIEW OUR MENU
                    <i class="fa-solid fa-circle-arrow-right"></i>
                </a>

            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;

.row {
    padding-top: 17rem;
    padding-bottom: 25rem;

    p {
        color: $brand_primary;
        font-size: 3rem;
        font-weight: 500;
        margin-bottom: 0;
    }

    h1 {
        font-size: 5.1rem;
        font-weight: 700;
        color: $brand_primary;
        margin-bottom: 1rem;

        span {
            color: $brand_secondary;
        }

    }

    a {
        background-color: $brand_tertiary;
        padding: .5rem 1.5rem;
        font-size: .9rem;
        font-weight: 500;

        i {
            margin-left: .7rem;
        }
    }


}
</style>