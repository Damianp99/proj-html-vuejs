<template>
  <div class="bottom-footer text-secondary">
    <div class="container d-flex justify-content-between align-items-center">
      <ul>
        <li v-for="infomation in informations" :key="infomation.text">
          <img
            class="logo-footer"
            :src="require(`../assets/images/${infomation.img}`)"
            alt="logo porto"
          />
          <span>{{ infomation.text }}</span>
        </li>
      </ul>

      <ul>
        <li v-for="link in links" :key="link.text">
          <a class="text-muted small" :href="link.url">
            <font-awesome-icon
              icon="fa-solid fa-chevron-right "
              class="px-1"
            />{{ link.text }}</a
          >
        </li>
        <li />
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "BottomFooter",
  props: ["informations", "links"],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
*a {
  text-decoration: none;
}
</style>