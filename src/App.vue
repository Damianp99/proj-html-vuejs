<template>
  <div id="app">
    <Header :upperlinks="upper_menu" :bottomlinks="bottom_menu" />
    <Main />
    <UpperFooter
      :blog="blog"
      :post="recentPost"
      :comments="recentComments"
      :categories="categories"
    />
    <BottomFooter :informations="footer_left" :links="footer_right" />
  </div>
</template>

<script>
import BottomFooter from "./components/BottomFooter.vue";
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import UpperFooter from "./components/UpperFooter.vue";
export default {
  name: "App",
  components: {
    Header,
    Main,
    UpperFooter,
    BottomFooter,
  },
  data() {
    return {
      upper_menu: [
        { text: "Sign In", url: "#" },
        { text: "About Us", url: "#" },
        { text: "Contact Us", url: "#" },
        { text: "Buy Now", url: "#" },
      ],
      bottom_menu: [
        { text: "Home", url: "#" },
        { text: "Elements", url: "#" },
        { text: "Features", url: "#" },
        { text: "Pages", url: "#" },
        { text: "Portofolio", url: "#" },
        { text: "Blog", url: "#" },
        { text: "Shop", url: "#" },
      ],

      blog: {
        title: "ABOUT THE BLOG",
        text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.Lorem ipsum dolor sit amet",
        more_text:
          "Lorem ipsum dolor sit amet consectetur adipisicing elit.Lorem ipsum dolor sit amet",
        view_more: "VIEW MORE",
      },
      recentPost: {
        title: "RECENT POSTS",
        text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        more_text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        date: "12:53 AM Dec 19th",
        url: "our-office-4-square.jpg",
        another_url: "our-office-5-square.jpg",
      },
      recentComments: {
        title: "RECENT COMMENTS",
        text: "John Doe commented lorem ipsum dolor sit amet",
        more_text: "John Doe commented lorem ipsum dolor sit amet",
        more: "VIEW MORE",
        date: "12:55 AM Dec 19th",
      },
      categories: [
        { text: "GADGETS", url: "#" },
        { text: "PHOTOGRAPHY", url: "#" },
        { text: "LIFESTYLE", url: "#" },
        { text: "FASHION", url: "#" },
        { text: "RECIPES", url: "#" },
        { text: "TRAVEL", url: "#" },
        { text: "BUSINESS", url: "#" },
        { text: "ARCHITECTURE", url: "#" },
        { text: "REVIEWS", url: "#" },
        { text: "SPORTS", url: "#" },
        { text: "VIDEOS", url: "#" },
        { text: "TECHNOLOGY", url: "#" },
        { text: "DESIGN", url: "#" },
      ],

      footer_left: [
        {
          text: "Copyright 2020. All Rights Reserved",
          img: "logo-footer.png",
        },
      ],
      footer_right: [
        {
          text: "FAQ's",
          url: "#",
        },
        {
          text: "Sitemap",
          url: "#",
        },
        {
          text: "Contact Us",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
