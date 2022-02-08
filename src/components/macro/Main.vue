<template>
    <main class="container">
        <Services />
        <AvadaProducts />
        <FeaturedProduct />
    </main>
</template>

<script>
import Services from '../section/Services.vue'
import AvadaProducts from '../section/AvadaProducts.vue'
import FeaturedProduct from '../section/FeaturedProduct.vue'

export default {
    name: 'Main',
    props: {},
    components: {
        Services,
        AvadaProducts,
        FeaturedProduct,
    },
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

</style>