<template>
    <main class="container">
        <!-- <elem /> -->
        {{msg}}
    </main>
</template>

<script>
//import elem from '../section/elem.vue'

export default {
    name: 'Main',
    props: {
        msg: String,
    },
    components: {
        //elem,
    },
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
</style>