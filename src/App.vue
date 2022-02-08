<template>
  <div id="app">
    <Header />
    <HeaderTail />
    <Main />

    <Footer />
  </div>
</template>

<script>
import Main from "./components/macro/Main.vue";
import Footer from "./components/macro/Footer.vue";
import Header from "./components/macro/Header.vue";
import HeaderTail from "./components/section/HeaderTail.vue";

export default {
  name: "App",
  data() {
    return {};
  },
  methods: {},
  components: {
    Main,
    Footer,
    Header,
    HeaderTail,
  },
};
</script>

<style lang="scss">
@import "./assets/style/globals.scss";

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
