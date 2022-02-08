<template>
    <div id="" class="footer-image">
        <div class="image">
            <img :src="require('../../assets/img/Footer/' + thumb)" alt="">
        </div>
        <Button :msg="buttonMsg"/>
    </div>
</template>

<script>
import Button from '../common/Button.vue'

export default {
    name: "FooterImage",
    components: {
        Button,
    },
    data(){
        return{}
    },
    props: {
        buttonMsg: String,
        thumb: String,
    },
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
.footer-image{
    text-align: center;
}

img{
    width: 300px;
}
</style>