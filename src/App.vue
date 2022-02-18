<template>
  <div id="app">
    <Header :links="links" />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
  data() {
    return {
      links: [
        {
          upper_menu: ["Sign In", "About Us", "Contact Us", "Buy Now"],
          bottom_menu: [
            "Home",
            "Elements",
            "Features",
            "Pages",
            "Portofolio",
            "Blog",
            "Shop",
          ],
          footer: [""],
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
