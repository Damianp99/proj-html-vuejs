<template>
  <main>
    <Jumbo />
    <Posts />
  </main>
</template>

<script>
import Jumbo from "./Jumbo.vue";
import Posts from "./Posts.vue";
export default {
  name: "Main",
  components: {
    Jumbo,
    Posts,
  },
  props: [""],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
</style>