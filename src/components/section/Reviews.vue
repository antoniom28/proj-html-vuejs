<template>
    <div id="reviews" class="">
        <div class="title">
            <span>WHAT PEOPLE SAY</span>
            <h1>Reviews</h1>
        </div>
        <div class="reviews-box">
            <BoxThumbTitle 
                v-for="(data,index) in dataReviews"
                :key="index"
                :data="data"
                type="reviews"
            />
        </div>
    </div>
</template>

<script>
import BoxThumbTitle from '../common/BoxThumbTitle.vue'
import AllData from '../../assets/data/AllData.json'

export default {
    name: "Reviews",
    data(){
        return{
            dataReviews: AllData.reviews, 
        }
    },
    components: {
        BoxThumbTitle,
    },
    props: {},
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
#reviews{
    text-align: center;
    padding-bottom: 110px;
}

#reviews > *{
    margin: 50px 0;
}

.reviews-box{
    padding: 0 180px;
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