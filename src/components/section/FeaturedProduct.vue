<template>
    <div class="featured-product">
        <div class="special-product">
            <div class="thumb">
                <img src="../../assets/img/Main/shaving_butter.png" alt="">
            </div>
            <div class="text">
                <p>THIS MONTHS FEATURE PRODUCT</p>
                <h2>Shaving Butter</h2>
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

.special-product{
    background-color: $cube_1;
    border-top: 3px solid $text_color;
    display: flex;
    width: 880px;
    margin: 0 auto;
    transform: translateY(-50px);
}

.thumb{
    background-image: url(../../assets/img/Main/avadabarbers-cta-background.jpg);
    background-size: cover;
    width: 30%;
        position: relative;

    img{
        width: 80%;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%,-50%);
    }
}

.text{
    width: 70%;
    text-align: start;
    padding: 40px 25px;

    p{
        color: $text_color;
        font-size: 0.9em;
    }

    h2{
        color: $text_2_color;
    }

    span{
        color: $text_3_color;
        display: inline-block;
        margin: 20px 0 5px 0;
    }
}


</style>