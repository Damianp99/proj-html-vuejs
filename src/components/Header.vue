<template>
  <header>
    <div class="upper-header text-white">
      <div class="container">
        <ul class="list-unstyled d-flex align-items-center">
          <li class="small text-light-blue">
            Everything about Lifestyle,Travel and Gadgets
          </li>
          <li v-for="(link, i) in links" :key="i">
            {{ link.upper_menu }}
          </li>
        </ul>
      </div>
    </div>
    <div class="container">
      <div class="mid-header">
        <img src="../assets/images/logo-default-slim.png" alt="Logo Porto" />
      </div>
    </div>
    <div class="bottom-header container">
      <div class="d-flex justify-content-between align-items-center">
        <ul class="list-unstyled bottom-list">
          <li v-for="(link, i) in links" :key="i">
            {{ link.bottom_menu }}
          </li>
        </ul>
        <div>
          <i class="fa-solid fa-magnifying-glass"></i>
          <input type="text" />
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  components: {},
  props: ["links"],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
i {
  width: 20px;
}
</style>