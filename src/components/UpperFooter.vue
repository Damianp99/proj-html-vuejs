<template>
  <footer>
    <div class="upper-footer d-flex py-5 small">
      <div class="d-flex container">
        <div class="col-3 text-white blog">
          <h4 class="">{{ blog.title }}</h4>
          <p class="text-secondary">{{ blog.text }}</p>
          <p class="text-secondary">{{ blog.more_text }}</p>
          <span>{{ blog.more }}</span>
          <span class="fw-bold small">
            {{ blog.view_more
            }}<font-awesome-icon icon="fa-solid fa-chevron-right " class="ps-1"
          /></span>
        </div>
        <div class="col-3 text-white post">
          <h4 class="">{{ post.title }}</h4>

          <div class="d-flex">
            <img
              :src="require(`../assets/images/${post.url}`)"
              alt="post picture"
            />

            <p class="p-1">
              {{ post.text }} <br />
              <span class="text-secondary"> {{ post.date }}</span>
            </p>
          </div>
          <div class="d-flex">
            <img
              :src="require(`../assets/images/${post.another_url}`)"
              alt="post picture"
            />

            <p class="p-1">
              {{ post.more_text }} <br />
              <span class="text-secondary">{{ post.date }}</span>
            </p>
          </div>
        </div>
        <div class="col-3 text-white comments">
          <h4 class="">{{ comments.title }}</h4>

          <p>
            <font-awesome-icon
              icon="fa-solid fa-chevron-right "
              class="px-1"
            />{{ comments.text }}
            <span class="text-secondary">{{ comments.date }}</span>
          </p>

          <p>
            <font-awesome-icon icon="fa-solid fa-chevron-right " />
            {{ comments.more_text }}
            <span class="text-secondary">{{ comments.date }}</span>
          </p>
        </div>
        <div class="col-3 text-white categories">
          <h4 class="">CATEGORIES</h4>
          <button
            class="btn bg-black btn-black m-1 rounded"
            v-for="categorie in categories"
            :key="categorie.text"
          >
            {{ categorie.text }}
          </button>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  components: {},
  props: ["blog", "post", "comments", "categories"],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
h4 {
  font-size: 14px;
}
.btn-black {
  font-size: 14px;
  padding: 5px;
  font-size: 10px;
  font-weight: 600;
}

.post {
  img {
    width: 70px;
    height: 70px;
    border-radius: 50%;
  }
}
</style>