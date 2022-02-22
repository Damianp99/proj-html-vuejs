<template>
  <div>
    <div class="card d-flex justify-content-between">
      <img src="../assets/images/blog-54.jpg" alt="card picture" />

      <div class="col-12 d-flex justify-content-between">
        <div class="d-flex flex-column me-3">
          <span class="bg-white text-black p-1">12</span>
          <span class="bg-onyx text-white p-1">Jan</span>
        </div>
        <div>
          <h2 class="text-capitalized">how to make friends as a grown-up</h2>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi
            modi, praesentium iusto quaerat id officiis dolore incidunt iste,
            dignissimos aperiam autem perspiciatis laudantium distinctio! Dicta
            aut exercitationem vero voluptatum quaerat!
          </p>
          <div class="d-flex justify-content-between">
            <ul>
              <li>
                <font-awesome-icon icon="fa-solid fa-user" />By<a href=""
                  >John Doe</a
                >
              </li>
              <li>
                <font-awesome-icon icon="fa-solid fa-folder" /><a href=""
                  >Lifestyle,Travel</a
                >
              </li>
              <li>
                <font-awesome-icon icon="fa-solid fa-comments" /><a href=""
                  >12 Comments</a
                >
              </li>
            </ul>
            <button class="btn text-muted small me-3">READ MORE</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Cards",
};
</script>

<style lang="scss" scoped>
</style>