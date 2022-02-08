<template>
    <div id="" class="button">
        <a href="#" class="classic-button">
            {{msg}}
        </a>
    </div>
</template>

<script>
export default {
    name: "Button",
    data(){
        return{}
    },
    props: {
        msg: String,
    },
    methods: {},
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
.classic-button{
    display: inline-block;
    border: 2px solid $text_color;
    color: $text_color;
    font-weight: 300;
    font-size: 1.1em;
    padding: 7px 20px;
}
</style>