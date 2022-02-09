<template>
    <header class="container">
        <HeaderMenu />

        <div class="header-ads">
            <div class="demos">
                <i class="fas fa-id-badge"></i>
                <p>Demos</p>
            </div>
            <div class="sale">
                <div class="dollar">
                    <i class="fas fa-dollar-sign"></i>
                    <span>39</span>
                </div>
                <p>On Sale</p>
            </div>
        </div>

        <HeaderMainBox />

    </header>
</template>

<script>
import HeaderMenu from '../section/HeaderMenu.vue'
import HeaderMainBox from '../section/HeaderMainBox.vue'

export default {
    name: 'Header',
    components: {
        HeaderMenu,
        HeaderMainBox,
    },
    props: {},
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

header{
    min-height: 100vh;
    background-image: url("../../assets/img/Header/avadabarbers-homepage-hero-bg.jpg");
    background-size: cover;
}

.header-ads{
    position: absolute;
    right: 12px;
    top: 90px;


    p{
        font-size: 0.7em;
    }

    .demos,.sale{
        background-color: white;
        margin: 5px 0;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 60px;
        height: 60px;
        border-radius: 10px;
    }

    .dollar{
        color: green;
        font-weight: bold;
    }
    .fa-dollar-sign{
        font-size: 0.7em;
        transform: translateY(-5px)
    }
}

    /*ul{
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 300px;

        li{
            cursor: pointer;
            color: $text_color;

            &:hover{
                color:$text_2_color;
            }
        }
    }*/
</style>