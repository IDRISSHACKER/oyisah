<template>
  <div class="container">
    <div class="blocs mt mb">
        <div>
          <bloc-widget
            title="Construisez et expédiez plus rapidement à l'aide d'outils simples"
            content="Tous nos produits sont construits avec la simplicité à la base,
            vous pouvez donc passer votre temps à vous concentrer sur la création d'applications,
            et non sur l'infrastructure."
           img="https://www.digitalocean.com/_next/static/media/bar-chart.656d9366.png"
          />
        </div>
        <div>
          <bloc-widget
            title="Réduisez vos obstacles grâce à un support dédié"
            content="énéficiez d'une assistance gratuite et personnalisée ou passez à des plans
            payants pour recevoir une aide dédiée et des temps de réponse plus rapides."
            img="https://www.digitalocean.com/_next/static/media/speech-bubbles.cc4ac392.png"
          />
        </div>
    </div>
  </div>
</template>
<script lang="ts">
import {defineComponent} from "vue";
import BlocWidget from "components/widget/bloc.vue";

export default defineComponent({
  name: "BlocksWidget",
  components: {BlocWidget}
})
</script>
<style lang="scss">
  .blocs{
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 40px;
  }
</style>
