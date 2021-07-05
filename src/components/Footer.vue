<template>
  <div class="container-footer">
    <div class="footer-main">
      <div>
        <h3>Links</h3>
        <ul>
          <li><fa icon="angle-right" /><a href="#">Location</a></li>
          <li><fa icon="angle-right" /><a href="#">Products</a></li>
          <li><fa icon="angle-right" /><a href="#">Home</a></li>
          <li><fa icon="angle-right" /><a href="#">About-us</a></li>
        </ul>
      </div>
      <div>
        <h3>Social</h3>
        <ul>
          <li>
            <a href="#"><fa :icon="['fab', 'facebook-square']" /> Facebook</a>
          </li>
          <li>
            <a href="#"><fa :icon="['fab', 'instagram-square']" /> Instagram</a>
          </li>
          <li>
            <a href="#"><fa :icon="['fab', 'twitter-square']" /> Twitter</a>
          </li>
          <li>
            <a href="#"><fa :icon="['fab', 'whatsapp-square']" /> Whatsapp</a>
          </li>
        </ul>
      </div>
      <div>
        <h3>Contact</h3>
        <ul class="footer-locations">
          <li>
            <fa icon="envelope" /><a href="mailto:adm@coffeshop.com.br"
              >adm@coffeshop.com.br</a
            >
          </li>
          <li>
            <fa icon="phone-alt" /><a href="tel:+440-540-6348"
              >Tel: 440-540-6348</a
            >
          </li>
          <li>
            <fa icon="map-marker-alt" />
            <a
              href="http://maps.google.com/?q=1200 Pennsylvania Ave SE, Washington, District of Columbia, 20003"
              target="_blank"
            >
              Address: 2952 Bingamon Road asdasdasd asd asd</a
            >
          </li>
        </ul>
      </div>
    </div>
    <div class="footer-bottom">
      <p>
        <a href="https://github.com/henriquemod" target="_blank"
          >2021 - Made by Henrique Souza</a
        >
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style src="../assets/css/style.css"/>