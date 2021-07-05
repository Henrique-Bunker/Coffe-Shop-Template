<template>
  <div class="container-home-review">
    <Carousel
      :items-to-show="totalReviewsOnScreen"
      :wrap-around="true"
      :autoplay="1"
      :transition="5000"
    >
      <Slide v-for="review in reviewSlides" :key="review">
        <div class="carousel__reviews">
          <img :src="review[1]" alt="" />
          <div class="review-item">
            <h2>{{ review[0] }}</h2>
            <p>"{{ review[2] }}"</p>
          </div>
        </div>
      </Slide>
    </Carousel>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import { Carousel, Slide } from "vue3-carousel";

import "vue3-carousel/dist/carousel.css";

const totalReviewsOnScreen = 3;

const reviewSlides = [
  ["Keanu", "/assets/img/profile1.jpg", "The best coffe shop in the world!"],
  ["Keanu2", "/assets/img/profile1.jpg", "The best coffe shop in the world!"],
  ["Keanu", "/assets/img/profile1.jpg", "The best coffe shop in the world!"],
  ["Keanu2", "/assets/img/profile1.jpg", "The best coffe shop in the world!"],
];

export default defineComponent({
  name: "HomeReview",
  components: {
    Carousel,
    Slide,
  },
  mounted() {
    window.addEventListener("resize", () => {
      if (window.innerWidth < 900) {
        this.totalReviewsOnScreen = 2;
      } else if (window.innerWidth < 600) {
        this.totalReviewsOnScreen = 1;
      } else {
        this.totalReviewsOnScreen = 3;
      }
    });
  },
  data() {
    return {
      reviewSlides,
      totalReviewsOnScreen,
    };
  },

  computed: {},
});
</script>

<style src="../../assets/css/style.css"/>