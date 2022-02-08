<template>
    <footer>
        <div class="container">
            <FooterImage 
                thumb="avadabarbers_footer_shop_image.png"
                buttonMsg="SHOP OUR RANGE NOW"
            />
            <FooterInfo :info="barberInfo"/>
            <FooterImage 
                thumb="avadabarbers_footer_appointment_image.png"
                buttonMsg="BOOK YOUR APPOINTMENT"
            />
        </div>

        <div  class="copyright-box">
            <span class="copyright">
                <i class="far fa-copyright"></i>
                Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress
            </span>
        </div>
    </footer>
</template>

<script>
import FooterImage from '../section/FooterImage.vue'
import FooterInfo from '../section/FooterInfo.vue'
import AllData from '../../assets/data/AllData.json'

export default {
    name: 'Footer',
    components: {
        FooterImage,
        FooterInfo
    },
    data(){
        return{
            barberInfo: AllData.yourInfo,
        }
    },
    props: {},
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
footer{
    background-color: $cube_1;
}

.container{
    padding: 20px 30px;
    display: flex;
    justify-content: space-around;
   align-items: center;
    flex-wrap: wrap;
}

.copyright-box{
    text-align: center;
    padding: 35px 0;
    width: 100%;
    background-color: $median_1;
    color: $text_3_color;
}
</style>