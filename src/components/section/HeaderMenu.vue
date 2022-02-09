<template>
    <div id="" class="header-menu">
        <div v-if="!menu">
            <a href="#">
                <img src="../../assets/img/Header/avadabarbers-logo-x1.png" alt="">
            </a>
        </div>

        <div  v-if="!menu" class="main-nav">
            <div class="shop">
                <i class="fas fa-shopping-cart shop-icon"></i>
            </div>
            <div @click="showMenu(true)" class="hidden-menu">
                <i class="fas fa-bars menu-icon"></i>
            </div>
        </div>

         <nav v-if="menu">
            <ul>
                <li><img src="../../assets/img/Header/avadabarbers-logo-x1.png" alt=""></li>
                <li @click="showMenu(false)">
                    <a href="#">HOME</a>
                </li>
                <li
                    @click="showMenu(false)"
                    v-for="(elem,index) in menuItem"
                    :key="index"
                >
                    <a :href="'#' + elem"> {{elem.charAt(0).toUpperCase() + elem.slice(1)}} </a>
                </li>
            </ul>
        </nav> 
    </div>
</template>

<script>
export default {
    name: "HeaderMenu",
    data(){
        return{
           menu : false,
           menuItem: ['services','products','reviews','blog','info'],
        }
    },
    props: {},
    methods: {
        showMenu(bool){
            this.menu = bool;
        },
        getScroll(){
            let scroll = document.documentElement.scrollTop;
            console.log(scroll);
        }
    },
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
ul{
    width: 80%;
    height: 80px;
    color: $text_2_color;
    display: flex;
    justify-content: space-around;
    align-items: center;
    position: absolute;
    top: -80px;
    left: 10%;
    animation: slideTop 0.2s linear forwards;

    li a{
        color: $text_2_color;
    }
}

@keyframes slideTop {
    to{
        top: 0px;
    }
}

.header-menu{
    height: 80px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 60%;
    margin: 0 auto;
    position: relative;

    img{
        width: 140px;
    }
}

.main-nav{
    width: 60px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: white;

    .menu-icon{
        cursor: pointer;
        font-size: 1.5em;
    }
}
</style>