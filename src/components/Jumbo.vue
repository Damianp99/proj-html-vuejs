<template>
  <div>
    <div class="row">
      <div
        id="jumbotron"
        class="col-4"
        v-for="(jumbotron, i) in jumbotrons"
        :key="i"
        :style="{
          backgroundImage: 'url(' + jumbotron.url + ')',
        }"
      >
        <button class="btn btn-blue">
          {{ jumbotron.buttonText }}
        </button>
        <h5 class="text-capitalize">{{ jumbotron.text }}</h5>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Jumbo",
  data() {
    return {};
  },
  props: ["jumbotrons"],
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/style.scss";
#jumbotron {
}
</style>