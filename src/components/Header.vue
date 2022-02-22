<template>
  <header>
    <div class="upper-header text-white">
      <div class="container">
        <ul class="list-unstyled d-flex align-items-center">
          <li class="small text-light-blue">
            Everything about Lifestyle,Travel and Gadgets
          </li>
          <li v-for="upperlink in upperlinks" :key="upperlink.text">
            <a class="text-white small" :href="upperlink.url">{{
              upperlink.text
            }}</a>
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
          <li v-for="bottomlink in bottomlinks" :key="bottomlink.text">
            <a class="text-dark fw-bolder" :href="bottomlink.url">{{
              bottomlink.text
            }}</a>
          </li>
        </ul>
        <div class="search-bar">
          <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
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
  props: ["bottomlinks", "upperlinks"],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
i {
  width: 20px;
}
*a {
  text-decoration: none;
}
input {
  border: 1px solid darkgray;
  border-top: 0;
  border-right: 0;
  border-bottom: 0;
}
.search-bar {
  position: relative;
}
.fa-magnifying-glass {
  position: absolute;
  top: 50%;
  left: 10%;
  transform: translate(-50%, -50%);
}
</style>