<template>
    <div id="" class="header-menu">
        <div>
            <a href="#">
                <img src="../../assets/img/Header/avadabarbers-logo-x1.png" alt="">
            </a>
        </div>

        <div class="main-nav">
            <div class="shop">
                <i class="fas fa-shopping-cart shop-icon"></i>
            </div>
            <div class="hidden-menu">
                <i class="fas fa-bars menu-icon"></i>
            </div>
        </div>
        <!-- <nav>
            <ul>
                <li
                    v-for="(elem,index) in menuItem"
                    :key="index"
                >
                    {{elem}}
                </li>
            </ul>
        </nav> -->
    </div>
</template>

<script>
export default {
    name: "HeaderMenu",
    data(){
        return{}
    },
    props: {},
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
.header-menu{
    height: 80px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 300px;

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