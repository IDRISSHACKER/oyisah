<template>
  <div class="container">
    <o-card
      title="Créez des boutiques et des sites Web de commerce électronique
            de manière transparente"
      desc="Laissez les tracas de la gestion d'un site Web aux experts.
            Inscrivez-vous maintenant à l'hébergement géré  et obtenez 2000 xaf de crédit gratuit.
          "
      img-link="https://www.digitalocean.com/_next/static/media/lighthouse-clouds-blue.8a1f1a95.svg"
      link-text="Commencer mon essai gratuit"/>
  </div>
</template>
<script lang="ts">
import {defineComponent} from "vue";
import OCard from "components/cards/ocard.vue";

export default defineComponent({
  name: "shopApp",
  components: {OCard}
})
</script>
