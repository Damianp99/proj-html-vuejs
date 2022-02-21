<template>
  <main>
    <div class="bg-jumbotron mb-5">
      <div class="container d-flex align-items-center flex-wrap g-3 py-3">
        <Jumbo :jumbotrons="jumbotrons" />
      </div>
    </div>

    <div class="container">
      <div class="row">
        <div class="col-4">
          <h5 class="fw-bolder small">POPULAR POSTS</h5>
          <Posts :popularPosts="popularPosts" />
        </div>
        <div class="col-4">
          <h5 class="fw-bolder small">RECENT POSTS</h5>
          <Posts :recentPosts="recentPosts" />
        </div>
        <div class="col-4">
          <h5 class="fw-bolder small">FEATURED POST</h5>
          <div>
            <h5 class="fw-bolder small">FEATURED AUTHOR</h5>
          </div>
        </div>
      </div>
    </div>

    <Slider />
    <div class="container">
      <div class="row">
        <div class="col-8">
          <Cards />
        </div>
        <div class="col-4"></div>
      </div>
    </div>
  </main>
</template>

<script>
import Slider from "./Slider.vue";
import Cards from "./Cards.vue";
import Jumbo from "./Jumbo.vue";
import Posts from "./Posts.vue";
export default {
  name: "Main",
  components: {
    Jumbo,
    Posts,
    Slider,
    Cards,
  },
  props: [""],
  data() {
    return {
      popularPosts: [
        {
          url: "blog-55.jpg",
          text: "Simple Ways To Have A Pretty Face",
          date: "January 12, 2019",
        },
        {
          url: "blog-56.jpg",
          text: "ranking the greatest players in basketball",
          date: "January 12, 2019",
        },
        {
          url: "blog-57.jpg",
          text: "4 ways to look cool in glasses",
          date: "January 12, 2019",
        },
        {
          url: "blog-58.jpg",
          text: "top camper trailer towing tips",
          date: "January 12, 2019",
        },
        {
          url: "blog-59.jpg",
          text: "5 lovely walks in new york",
          date: "January 12, 2019",
        },
      ],
      recentPosts: [
        {
          url: "blog-65.jpg",
          text: "main reasons to stop texting and driving",
          date: "January 12, 2019",
        },
        {
          url: "blog-66.jpg",
          text: "tips to help you quickly prepare your lunch",
          date: "January 12, 2019",
        },
        {
          url: "blog-67.jpg",
          text: "why should i buy a smartwatch",
          date: "January 12, 2019",
        },
        {
          url: "blog-68.jpg",
          text: "the best augmented reality smartglasses",
          date: "January 12, 2019",
        },
        {
          url: "blog-69.jpg",
          text: "12 healthiest foods to eat for breakfast",
          date: "January 12, 2019",
        },
      ],
      jumbotrons: [
        {
          url: "..assets/images/blog-46.jpg",
          text: "how to take a better concert pictures in 30 seconds",
          buttonText: "PHOTOGRAPHY",
        },
        {
          url: "..assets/images/blog-47.jpg",
          text: "gadgets that make your smartphone even smarter",
          buttonText: "GADGETS",
        },
        {
          url: "..assets/images/blog-48.jpg",
          text: "20 top-rated tourist attractions in manhattan",
          buttonText: "TRAVEL",
        },
        {
          url: "..assets/images/blog-49.jpg",
          text: "the best way to ride a motorcycle",
          buttonText: "LIFESTYLE",
        },
        {
          url: "..assets/images/blog-50.jpg",
          text: "5 fun things to do at the beach",
          buttonText: "TRAVEL",
        },
        {
          url: "..assets/images/blog-51.jpg",
          text: "amazingly fresh fruit and herb drinks for summer",
          buttonText: "RECIPES",
        },
      ],
      featured: {
        featuredPosts: {},
        featuredAuthor: {
          url: "..assets/images/avatar.jpg",
          author: "John Doe",
          text: "lorem ipsum",
        },
      },
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
</style>