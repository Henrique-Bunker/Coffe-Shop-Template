<template>
  <Carousel :autoplay="2500" :wrap-around="true" :transition="2500">
    <Slide v-for="slide in imgSlides" :key="slide">
      <div class="carousel__item">
        <img :src="slide" alt="" srcset="" />
      </div>
    </Slide>
  </Carousel>
</template>

<script>
import { defineComponent } from "vue";
import { Carousel, Slide } from "vue3-carousel";

const imgSlides = [
  "/assets/img/slide2.jpg",
  "/assets/img/slide1.jpg",
  "/assets/img/slide3.jpg",
  "/assets/img/slide4.jpg",
];

export default defineComponent({
  name: "Basic",
  components: {
    Carousel,
    Slide,
  },
  data() {
    return {
      imgSlides,
    };
  },
});
</script>

<style src="../assets/css/style.css"/>
