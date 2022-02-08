<template>
    <div id="" class="header-tail">
        <div class="pro-barber">
            <span>AWARD WINNING</span>
            <h1>Pro Barbers</h1>
            <Button msg="MEET YOUR NEW BARBER"/>
        </div>
    <Median class-color="color-0 top"/>
    </div>
</template>

<script>
import Button from '../common/Button.vue'
import Median from '../common/Median.vue'

export default {
    name: "HeaderTail",
    data(){
        return{}
    },
    components: {
        Button,
        Median,
    },
    props: {},
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
.header-tail{
    background-image: url("../../assets/img/Header/avadabarbers-about-introbackground.jpg");
    background-size: cover;
    text-align: center;
}

.pro-barber{
    display: inline-block;
    margin: 100px 0;
}

span{
    color: $text_color;
    font-size: 0.8em;
}

h1{
    color: $text_2_color;
}
</style>