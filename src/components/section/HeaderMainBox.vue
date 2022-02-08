<template>
    <div id="" class="header-main-box">
        <div class="barber-shop">
            <h1>Barber Shop </h1>
            <hr>
            <span>The Pinnacle of Male Grooming</span>
            <br>
            <Button msg='LEARN MORE' />
        </div>

        <div class="image">
            <img src="../../assets/img/Header/avadabarbers_hero_focalmirror-600x825.png" alt="">
        </div>
    </div>
</template>

<script>
import Button from '../common/Button.vue'

export default {
    name: "HeaderMainBox",
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
.image img{
    width: 400px;
}

.barber-shop{
}

.header-main-box{
    //margin-left: 150px;
    display: flex;
    justify-content: center;
    align-items: center;

    > div{
        margin: 0 30px;
    }
}
.barber-shop *{
    margin: 15px 0;
}

h1{
    color: white;
    font-size: 3em;
}

hr{
    border: none;
    border-radius: 20px;
    height: 3px;
    width: 170px;
    background-color: $text_color;
}

span{
    color:$text_2_color;
}
</style>