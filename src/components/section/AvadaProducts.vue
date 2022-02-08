<template>
    <div id="products" class="">
        <Median classColor="color-1 top"/>
        <div class="title">
            <span>WE HAVE YOU COVERED</span>
            <h1>Avada Grooming Products</h1>
        </div>
        <div class="products-box">
            <BoxThumbTitle 
                v-for="(data,index) in dataProducts"
                :key="index"
                :data="data"
            />
        </div>
        <Button msg="SHOP OUR PRODUCT RANGE" />
    </div>
</template>

<script>
import Button from '../common/Button.vue'
import BoxThumbTitle from '../common/BoxThumbTitle.vue'
import AllData from '../../assets/data/AllData.json'
import Median from '../common/Median.vue'

export default {
    name: "AvadaProducts",
    data(){
        return{
            dataProducts: AllData.products, 
        }
    },
    components: {
        Button,
        BoxThumbTitle,
        Median,
    },
    props: {},
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
#products{
    text-align: center;
    background-image: url(../../assets/img/Main/avadabarbers-reviewsbackground.jpg);
    background-size: cover;
    padding-bottom: 160px;
}

#products > *:not(:first-child){
    margin-bottom: 50px;
}

.products-box{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
}

span{
    color: $text_color;
}

h1{
    color: $text_2_color;
}
</style>