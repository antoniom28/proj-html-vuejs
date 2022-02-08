<template>
    <div v-if="type != 'reviews'" id="" class="classic-box">
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

    <div v-else id="" class="classic-box">
        <span
            :class="data.textColor"
        >
            {{data.text}}
        </span>
        <img 
            :class="data.thumbSize"
            class="rounded"
            :src="require('../../assets/img/Main/' + data.thumb)" 
            alt=""
        >
        <span
            class="reviews"
            :class="data.titleColor"
        >
            {{data.name}}
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
        type: String,
    },
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

.classic-box{
    width: 300px;
}

span{
    display: inline-block;
}

.classic-box > *{
    margin: 15px 0;
}

.rounded{
    border-radius: 50px;
    display: block;
    margin: 0 auto;
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
img.s-medium{
    width: 180px;
}
img.medium{
    width: 280px;
}

h1{
    font-size: 2em;
}

//formati colore testo o altro, basta aggiungere gli altri quando sarà bisogno

.color-1{
    color: $text_color;
}
.color-2{
    color: $text_2_color;
}

</style>