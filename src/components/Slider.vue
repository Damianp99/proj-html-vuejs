<template>
  <div id="slider">
    <div class="container mt-5">
      <ul class="d-flex align-items-center justify-content-center p-4">
        <li><font-awesome-icon icon="fa-solid fa-chevron-left" /></li>
        <li>
          <button class="btn btn-black fw-bold text-white py-2 px-5">
            GADGETS
          </button>
        </li>
        <li>
          <button class="btn btn-black fw-bold text-white py-2 px-5">
            PHOTOGRAPHY
          </button>
        </li>
        <li>
          <button class="btn btn-black fw-bold text-white py-2 px-5">
            LIFESTYLE
          </button>
        </li>
        <li>
          <button class="btn btn-black fw-bold text-white py-2 px-5">
            FASHION
          </button>
        </li>
        <li>
          <button class="btn btn-black fw-bold text-white py-2 px-5">
            RECIPES
          </button>
        </li>
        <li>
          <button class="btn btn-black fw-bold text-white py-2 px-5">
            TRAVEL
          </button>
        </li>
        <li><font-awesome-icon icon="fa-solid fa-chevron-right" /></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Slider",
};
</script>

<style lang="scss" scoped>
button {
  font-size: 14px;
}
</style>