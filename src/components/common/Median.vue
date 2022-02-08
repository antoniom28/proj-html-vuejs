<template>
    <div id="" class="median" >
    <svg    
            :class="classColor"
            xmlns="http://www.w3.org/2000/svg" 
            width="100%" 
            height="100" 
            viewBox="0 0 100 100" 
            preserveAspectRatio="none" 
            style="padding:20px 0;"
        >
        <path d="M0 100 L50 2 L100 100 Z"/>
    </svg>
    </div>
</template>

<script>
export default {
    name: "Median",
    data(){
        return{}
    },
    props: {
        classColor: String,
    },
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
img{
    width: 100%;
    height: 100%;
}
.median{
 //   background-image: url("../../assets/img/triangle.svg");
    height: 80px;
}

.bottom{
    transform: rotate(180deg);
}

.color-0{
    fill: white; //bianco
}
.color-1{
    fill: $median_1; //circa nero
}
.color-2{
    fill: $median_2; //grigio scuro
}
.color-3{
    fill: $median_3; //grigio chiaro
}
.color-4{
    fill: $median_4; //un blu semi-chiaro
}
</style>