<template>
  <div>
    <div
      class="card d-flex justify-content-between"
      v-for="image in images"
      :key="image.url"
    >
      <img :src="require(`../assets/images/${image.url}`)" alt="card picture" />

      <div class="col-12 d-flex justify-content-between">
        <div class="d-flex flex-column me-3">
          <span class="bg-whitesmoke text-black p-1">12</span>
          <span class="bg-onyx text-white p-1">Jan</span>
        </div>
        <div>
          <h2 class="text-capitalize">{{ image.title }}</h2>
          <p>
            {{ image.text }}
          </p>
          <div class="d-flex justify-content-between py-2">
            <ul>
              <li>
                <font-awesome-icon
                  icon="fa-solid fa-user"
                  class="mx-2 icon-color"
                />By<a href="">John Doe</a>
              </li>
              <li>
                <font-awesome-icon
                  icon="fa-solid fa-folder"
                  class="mx-2 icon-color"
                /><a href="">Lifestyle,Travel</a>
              </li>
              <li>
                <font-awesome-icon
                  icon="fa-solid fa-comments"
                  class="mx-2 icon-color"
                /><a href="">12 Comments</a>
              </li>
            </ul>
            <button class="font-small btn-blank text-muted me-5">
              READ MORE
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Cards",
  props: ["images"],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
.card {
  border: 1px solid lightgray;
  border-left: 0px;
  border-right: 0px;
  border-radius: 0px;
}
img {
  height: 357px;
  object-fit: cover;
}
*a {
  text-decoration: none;
  font-size: 14px;
}
.icon-color {
  color: #b7b7b7;
}
.font-small {
  font-size: 12px;
}
</style>