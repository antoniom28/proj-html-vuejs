<template>
    <div id="info" class="footer-info">
        <div class="logo">
            <img src="../../assets/img/Footer/avadabarbers-logo-x1.png" alt="">
        </div>
        <div class="all-info">
            <p 
                v-for="(elem,index) in info"
                :key="index"
                class="info"
            >
                {{elem}}
            </p>
        </div>
        <p class="follow">FOLLOW US</p>
        <div class="social">
            <a href="#">
                <i class="fab fa-facebook-f"></i>
            </a>
            <a href="#">
                <i class="fab fa-twitter"></i>
            </a>
            <a href="#">
                <i class="fab fa-youtube"></i>
            </a>
            <a href="#">
                <i class="fab fa-instagram"></i>
            </a>
        </div>
    </div>
</template>

<script>
export default {
    name: "FooterInfo",
    data(){
        return{}
    },
    props: {
        info: Object,
    },
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
.footer-info{
    text-align: center;
}

.footer-info > *{
    margin: 35px 0;
}

img{
    width: 100px;
}

.info{
    color: $text_3_color;
}

.follow{
    color: $text_color;
}

a{
    color: $text_2_color;
}

.social > *{
    margin: 0 10px;
    font-size: 1.3em;
}
</style>