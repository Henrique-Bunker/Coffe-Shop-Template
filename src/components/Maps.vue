<template>
  <div class="container-map">
    <div class="local-image">
      <img src="../assets/img/local.jpg" alt="" />
    </div>
    <div class="googlemaps">
      <GoogleMap
        api-key="YOUR_GOOGLE_API_KEY"
        style="width: 100%; height: 100%"
        :center="center"
        :zoom="20"
      >
        <Marker :options="{ position: center }" />
      </GoogleMap>
    </div>
  </div>
</template>


<script>
import { defineComponent } from "vue";
import { GoogleMap, Marker } from "vue3-google-map";

export default defineComponent({
  name: "Maps",
  components: { GoogleMap, Marker },
  setup() {
    const center = { lat: 40.689247, lng: -74.044502 };

    return { center };
  },
});
</script>

<style src="../assets/css/style.css"/>