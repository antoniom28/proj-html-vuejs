<template>
    <div id="services" class="">
        <Median classColor="color-0 top"/>
        <div class="title">
            <span>MENS GROOMING</span>
            <h1>Services</h1>
        </div>
        <div class="services-box">
            <BoxThumbTitle 
                v-for="(data,index) in dataServices"
                :key="index"
                :data="data"
            />
        </div>
        <Button msg="READ ABOUT OUT SERVICES" />
    </div>
</template>

<script>
import Button from '../common/Button.vue'
import BoxThumbTitle from '../common/BoxThumbTitle.vue'
import AllData from '../../assets/data/AllData.json'
import Median from '../common/Median.vue'

export default {
    name: "Services",
    data(){
        return{
            dataServices: AllData.services, 
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
#services{
    text-align: center;
    padding-bottom: 160px;
}

#services > *:not(:first-child){
    margin-bottom: 50px;
}

.services-box{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 0 100px;
}

span{
    color: $text_color;
}

h1{
    color: $text_2_color;
}
</style>