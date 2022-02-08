<template>
    <div id="" class="median" >
    <svg    
            :class="classColor"
            xmlns="http://www.w3.org/2000/svg" 
            width="100%" 
            height="100%" 
            viewBox="0 0 100 100" 
            preserveAspectRatio="none" 
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
    height: 60px;
    transform: translateY(-60px);
}

.bottom{
    transform: rotate(180deg) translateY(-60px);
}

.color-0{
    fill: $cube_0; //bianco
}
.color-1{
    fill: $cube_1; //circa nero
}
.color-2{
    fill: $median_0; //grigio chiaro
}
</style>