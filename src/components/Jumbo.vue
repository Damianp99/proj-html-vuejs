<template>
  <div>
    <div class="row">
      <div
        id="jumbotron"
        class="col-4"
        v-for="(jumbotron, url) in jumbotrons"
        :key="url"
        :style="{
          backgroundImage: 'url(' + imagesUri + jumbotron.url + ')',
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
    return {
      imagesUri: "../assets/images/",
    };
  },
  props: ["jumbotrons"],
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/style.scss";
#jumbotron {
}
</style>