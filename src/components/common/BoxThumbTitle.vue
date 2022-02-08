<template>
    <div id="" class="classic-box">
        <img 
            :class="data.thumbSize"
            :src="require('../../assets/img/Main/' + data.thumb)" 
            alt=""
        >
        <h1
            :class="data.titleColor"
        >
            {{data.title}}
        </h1>
        <span
            :class="data.textColor"
        >
            {{data.text}}
        </span>
    </div>
</template>

<script>
export default {
    name: "BoxThumbTitle",
    data(){
        return{}
    },
    props: {
        data: Object,
    },
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

.classic-box > *{
    margin: 20px 0;
}

span{
    display: inline-block;
    width: 300px;
}

//formati immagine, basta aggiungere gli altri quando ci sarà bisogno
img{
    width: 100px;
}

img.e-small{
    width: 60px;
}
img.small{
    width: 80px;
}

h1{
    font-size: 2.5em;
}

//formati colore testo o altro, basta aggiungere gli altri quando sarà bisogno

.color-1{
    color: $text_color;
}
.color-2{
    color: $text_2_color;
}

</style>