<template>
  <div class="container">
    <o-card
      title="Visites guidées rapides des produits"
      desc="Consultez nos brèves visites de produits pour voir à quel point il est simple, facile et agréable d'utiliser
       les produits de DigitalOcean."
      img-link="https://www.digitalocean.com/_next/static/media/banner-background.f302a2e4.svg"
      link-text="Faire un tour"/>
  </div>
</template>
<script lang="ts">
import {defineComponent} from "vue";
import OCard from "components/cards/ocard.vue";

export default defineComponent({
  name: "kuikProduct",
  components: {OCard}
})
</script>
