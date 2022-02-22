<template>
  <footer>
    <div class="upper-footer d-flex py-5 small">
      <div class="d-flex container">
        <div class="col-3 text-white blog">
          <h4 class="">{{ blog.title }}</h4>
          <p>{{ blog.text }}</p>
          <p>{{ blog.more_text }}</p>
          <span>{{ blog.more }}</span>
          <span>{{ blog.view_more }}</span>
        </div>
        <div class="col-3 text-white post">
          <h4 class="">{{ post.title }}</h4>

          <div class="d-flex">
            <img
              :src="require(`../assets/images/${post.url}`)"
              alt="post picture"
            />

            <p>
              {{ post.text }} <br />
              <span>{{ post.date }}</span>
            </p>
          </div>
          <div class="d-flex">
            <img
              :src="require(`../assets/images/${post.another_url}`)"
              alt="post picture"
            />

            <p>
              {{ post.more_text }} <br />
              <span>{{ post.date }}</span>
            </p>
          </div>
        </div>
        <div class="col-3 text-white comments">
          <h4 class="">{{ comments.title }}</h4>

          <p>
            {{ comments.text }}
            <span>{{ comments.date }}</span>
          </p>

          <p>
            {{ comments.more_text }}
            <span>{{ comments.date }}</span>
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