<template>
  <main>
    <Jumbo />
    <Posts />
    <Slider />
  </main>
</template>

<script>
import Slider from "./Slider.vue";
import Jumbo from "./Jumbo.vue";
import Posts from "./Posts.vue";
export default {
  name: "Main",
  components: {
    Jumbo,
    Posts,
    Slider,
  },
  props: [""],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
</style>