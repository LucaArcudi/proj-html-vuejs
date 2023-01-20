<script>
export default {

}
</script>

<template >
    <section class="download">

        <div class="wrapper container-lg">
            <div class="row">
                <div class="col">
                    <p>Download Our</p>
                    <h1>
                        Ordering App
                    </h1>
                    <img src="../../assets/img/app-store-badge-200x67.png" alt="">
                    <img src="../../assets/img/play-store-badge-200x67.png" alt="">

                </div>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;


section.download {
    background-image: url(../../assets/img/app-ordering-scaled.jpg);
    background-size: cover;


    p {
        color: $brand_primary;
        font-size: 3rem;
        font-weight: 500;
        margin-bottom: 0;
        padding-top: 7rem;
    }

    h1 {
        font-size: 5.1rem;
        font-weight: 700;
        color: $brand_secondary;
        margin-bottom: 5rem;
    }

    img {
        margin-right: 2rem;
        margin-bottom: 9rem;
    }
}

div.row {
    margin-bottom: 10rem;
}
</style>