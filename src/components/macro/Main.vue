<template>
    <main class="container">
        <!-- <elem />
        

        <div class="pro-barber">
            <p>AWARD WINNING</p>
            <h2>Pro Barbers</h2>
            <a href="#" class="learn-button">
                MEET YOUR NEW BARBER
            </a>
        </div>
         -->
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