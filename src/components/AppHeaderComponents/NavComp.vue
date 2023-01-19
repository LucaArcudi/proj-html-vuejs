<script>
export default {
    data() {
        return {
            listItemList: ["Home", "Order Online", "About", "News", "Contact Us", `<i class="fa-solid fa-cart-shopping"></i>`]
        }
    },
}
</script>

<template >
    <section class="nav-section container-lg">
        <nav class="row justify-content-between">
            <div class="col-3">
                <img src="../../assets/img/takeout-logo.png" alt="">
            </div>
            <div class="col">
                <ul class="d-flex">
                    <li v-for="li in listItemList">{{ li }}</li>
                </ul>
            </div>
        </nav>
    </section>
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;

section.nav-section {
    padding-top: 5rem;

    ul {
        margin-top: 1rem;
        margin-bottom: 0;
        color: $brand_text_primary;
        list-style-type: none;
        justify-content: end;

        li {
            margin-left: 3rem;
            font-size: 1.2rem;
        }
    }
}
</style>