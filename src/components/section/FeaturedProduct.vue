<template>
    <div class="featured-product">
        <div class="special-product">
            <div class="thumb">
                <img src="../../assets/img/Main/shaving_butter.png" alt="">
            </div>
            <div class="text">
                <span>THIS MONTHS FEATURE PRODUCT</span>
                <h1>Shaving Butter</h1>
                <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                    Sint itaque nemo hic officiis consectetur, est, vero similique
                        accusamus fuga deserunt assumenda inventore deleniti in doloribus
                        architecto ea et incidunt eligendi.
                </span>
                <Button msg="BUY NOW" />
            </div>
        </div>
    </div>
</template>

<script>
import Button from '../common/Button.vue'

export default {
    name: "FeaturedProduct",
    data(){
        return{}
    },
    components: {
        Button,
    },
    props: {},
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

img{
    width: 100px;
}
</style>