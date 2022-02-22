<template>
  <div>
    <div class="card d-flex justify-content-between">
      <img
        v-for="collection in collections"
        :key="collection.url"
        :src="require(`../assets/images/${collection.url}`)"
        alt="card picture"
      />

      <div class="col-12 d-flex justify-content-between">
        <div class="d-flex flex-column me-3">
          <span class="bg-whitesmoke text-black p-1">12</span>
          <span class="bg-onyx text-white p-1">Jan</span>
        </div>
        <div>
          <h2 class="text-capitalize"></h2>
          <p></p>
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
  name: "Collection",
  props: ["collections"],
};
</script>

<style>
</style>