<template>
    <div id="" class="median" :class="classColor">
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
.median{
    background-image: url("../../assets/img/triangle.svg");
    height: 80px;
}

.bottom{
    transform: rotate(180deg);
}

.color-0{
    fill: $median_0;
}
.color-1{
    fill: $median_1;
}
.color-2{
    fill: $median_2;
}
.color-3{
    fill: $median_3;
}
.color-4{
    fill: $median_4;
}
</style>