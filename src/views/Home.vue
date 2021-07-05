<template>
  <div class="home">
    <div class="slider">
      <Slides />
    </div>
    <HomeBody />
    <div class="divider">Lorem ipsum</div>
    <HomeProducts />
    <div class="divider">Lorem ipsum</div>
    <HomeReview />
    <div class="divider">Lorem ipsum</div>
    <Maps />
  </div>
</template>

<script>
import Slides from "../components/Slides.vue";
import HomeBody from "../components/home/HomeBody.vue";
import HomeProducts from "../components/home/HomeProducts.vue";
import HomeReview from "../components/home/HomeReview.vue";
import Maps from "../components/Maps.vue";

export default {
  name: "Home",
  components: {
    Slides,
    HomeBody,
    HomeProducts,
    HomeReview,
    Maps,
  },
};
</script>

<style src="../assets/css/style.css"/>