<template>
    <main class="container">
        <Services />
        <AvadaProducts />
        <FeaturedProduct />
        <Reviews />
        <Blog />
    </main>
</template>

<script>
import Services from '../section/Services.vue'
import AvadaProducts from '../section/AvadaProducts.vue'
import FeaturedProduct from '../section/FeaturedProduct.vue'
import Reviews from '../section/Reviews.vue'
import Blog from '../section/Blog.vue'

export default {
    name: 'Main',
    props: {},
    components: {
        Services,
        AvadaProducts,
        FeaturedProduct,
        Reviews,
        Blog,
    },
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

</style>