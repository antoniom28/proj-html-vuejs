<template>
    <div id="blog" class="">
        <Median classColor="color-0 bottom" />
        <div class="title">
            <span>TALES FROM THE BARBER SHOP</span>
            <h1>Recent Blog Post</h1>
        </div>
        <div class="blog-box">
           <BoxThumbTitle 
                v-for="(data,index) in dataBlog"
                :key="index"
                :data="data"
            />
        </div>
        <Button msg="READ MORE FROM OUR BLOG"/>
    </div>
</template>

<script>
import BoxThumbTitle from '../common/BoxThumbTitle.vue'
import AllData from '../../assets/data/AllData.json'
import Button from '../common/Button.vue'
import Median from '../common/Median.vue'

export default {
    name: "Blog",
    data(){
        return{
            dataBlog: AllData.blog, 
        }
    },
    components: {
        BoxThumbTitle,
        Button,
        Median,
    },
    props: {},
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
#blog{
    text-align: center;
    background-color: $median_0;
    padding-bottom: 50px;
}

#blog > *{
    margin: 50px 0;
}

.blog-box{
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