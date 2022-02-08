<template>
    <main class="container">
        <Services />
    </main>
</template>

<script>
import Services from '../section/Services.vue'

export default {
    name: 'Main',
    props: {},
    components: {
        Services,
    },
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';
</style>