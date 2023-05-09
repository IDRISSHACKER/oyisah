<template>
  <div class="sources mt mb">
    <div class="soruces-head">
      <OcTitle
        title="Apprenez des experts"
        sub-title="Que vous souhaitiez en savoir plus sur le financement de votre entreprise,
          l'installation de Linux sur Ubuntu ou la mise en route de Oyisah,
          nous avons les ressources pédagogiques qu'il vous faut."
      />
    </div>
    <div class="container">
      <div class="sources-body">
        <simple-card
          title="Conseils aux entreprises"
          content="The Wave est la plaque tournante de Oyisah pour le
          contenu axé sur les startups et les entreprises sur le financement, l'embauche et la mise à l'échelle."
          img="https://www.digitalocean.com/_next/static/media/boat-storm-lighthouse.4bdddec0.png"
        />
        <simple-card
          title="Documentation produit"
          content="Découvrez comment faire tourner une machine virtuelle,
          démarrer avec le stockage par blocs et bien plus encore
           grâce à une documentation détaillée."
          img="https://www.digitalocean.com/_next/static/media/digitalocean-docs.26159f78.svg"
        />
        <simple-card
          title="Expertise technique"
          content="Visitez le site Web communautaire de Oyisah
          et CSS-Tricks pour apprendre à partir d'un large éventail de didacticiels techniques."
          img="https://www.digitalocean.com/_next/static/media/heart-speech-bubble-asterisk-graphic.6eb0678f.svg"
        />
      </div>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import OcTitle from "components/cards/ocTitle.vue";
import SimpleCard from "components/cards/simpleCard.vue";

export default defineComponent({
  name: "oSources",
  components: {SimpleCard, OcTitle}
})
</script>
<style lang="scss">
  .sources{
    .sources-body{
      margin-top: 100px;
      display: flex;
      align-items: baseline;
      justify-content: center;
      gap: 30px;
      flex-wrap: nowrap;
    }
  }
</style>
