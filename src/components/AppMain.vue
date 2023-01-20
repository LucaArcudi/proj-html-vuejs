<script>
import MostPopularComp from "./AppMainComponents/MostPopularComp.vue"
import MenuCategoriesComp from "./AppMainComponents/MenuCategoriesComp.vue"
import DownloadComp from "./AppMainComponents/DownloadComp.vue"
import NewsComp from "./AppMainComponents/NewsComp.vue"

export default {
    components: {
        MostPopularComp,
        MenuCategoriesComp,
        DownloadComp,
        NewsComp,
    }

}
</script>

<template>
    <main>
        <MostPopularComp />
        <MenuCategoriesComp />
        <DownloadComp />
        <NewsComp />
    </main>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
</style>