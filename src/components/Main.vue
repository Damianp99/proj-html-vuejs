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
        <div class="col-8 my-4">
          <Cards :images="cards" />
        </div>
        <div class="col-4">
          <SocialMedia />
        </div>
      </div>
      <div class="row">
        <div class="col-8">
          <Collection :collections="photoCollection" />
        </div>
      </div>
    </div>
  </main>
</template>

<script>
import SocialMedia from "./SocialMedia.vue";
import Collection from "./Collection.vue";
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
    SocialMedia,
    Collection,
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
          url: "blog-46.jpg",
          text: "how to take a better concert pictures in 30 seconds",
          buttonText: "PHOTOGRAPHY",
        },
        {
          url: "blog-47.jpg",
          text: "gadgets that make your smartphone even smarter",
          buttonText: "GADGETS",
        },
        {
          url: "blog-48.jpg",
          text: "20 top-rated tourist attractions in manhattan",
          buttonText: "TRAVEL",
        },
        {
          url: "blog-49.jpg",
          text: "the best way to ride a motorcycle",
          buttonText: "LIFESTYLE",
        },
        {
          url: "blog-50.jpg",
          text: "5 fun things to do at the beach",
          buttonText: "TRAVEL",
        },
        {
          url: "blog-51.jpg",
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
      photoCollection: {
        url: [
          "blog-13.jpg",
          "blog-16.jpg",
          "blog-20.jpg",
          "blog-23.jpg",
          "blog-29.jpg",
          "blog-40jpg",
        ],
        text: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Error id numquam hic provident reprehenderit harum, tempora earum repellendus totam beatae officia adipisci rerum dolor consequatur voluptas minus doloribus iste corrupti?",
      },
      cards: [
        {
          url: "blog-54.jpg",
          title: "How To Make Friends as a Grown-Up",
          text: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi modi, praesentium iusto quaerat id officiis dolore incidunt iste, dignissimos aperiam autem perspiciatis laudantium distinctio! Dicta aut exercitationem vero voluptatum quaerat!",
        },
        {
          url: "blog-55.jpg",
          title: "Simple Ways To Have A Pretty Face",
          text: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi modi, praesentium iusto quaerat id officiis dolore incidunt iste, dignissimos aperiam autem perspiciatis laudantium distinctio! Dicta aut exercitationem vero voluptatum quaerat!",
        },
        {
          url: "blog-56.jpg",
          title: "ranking the greatest players in basketball",
          text: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi modi, praesentium iusto quaerat id officiis dolore incidunt iste, dignissimos aperiam autem perspiciatis laudantium distinctio! Dicta aut exercitationem vero voluptatum quaerat!",
        },
        {
          url: "blog-58.jpg",
          title: "top camper trailer towing tips",
          text: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sequi modi, praesentium iusto quaerat id officiis dolore incidunt iste, dignissimos aperiam autem perspiciatis laudantium distinctio! Dicta aut exercitationem vero voluptatum quaerat!",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
</style>