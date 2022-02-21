<template>
  <div>
    <div
      class="d-flex flew-wrap post-border pt-2"
      v-for="(popularPost, index) in popularPosts"
      :key="index"
    >
      <img
        class="post-img me-2"
        :src="require(`../assets/images/${popularPost.url}`)"
        alt="post picture"
      />
      <div class="d-flex flex-column">
        <h6 class="text-capitalize fw-normal">{{ popularPost.text }}</h6>
        <div>
          <span class="text-muted small">{{ popularPost.date }}</span>
        </div>
      </div>
    </div>
    <div
      class="d-flex flew-wrap post-border pt-2"
      v-for="(recentPosts, index) in recentPosts"
      :key="index"
    >
      <img
        class="post-img me-2"
        :src="require(`../assets/images/${recentPosts.url}`)"
        alt="post picture"
      />
      <div class="d-flex flex-column">
        <h6 class="text-capitalize fw-normal">{{ recentPosts.text }}</h6>
        <div>
          <span class="text-muted small">{{ recentPosts.date }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Posts",
  props: ["popularPosts", "recentPosts", "featuredAuthor"],
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.post-border {
  padding-bottom: 10px;
  border-top: 0px;
  border-left: 0px;
  border-right: 0px;
  border-bottom: 1px solid lightgray;
  border-style: dotted;
}
.post-img {
  height: 50px;
  width: 50px;
}
.avatar {
  height: 100px;
  width: 100px;
}
</style>