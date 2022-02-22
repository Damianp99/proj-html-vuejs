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
          <a :href="link.url">{{ link.text }}</a>
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

<style>
</style>