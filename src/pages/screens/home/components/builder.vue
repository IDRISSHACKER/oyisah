<template>
  <div class="container">
    <div class="builder mt mb">
      <h3 class="title2 black center">Avantages de travailler avec oyisah</h3>
      <p class="text black-text center">
        Des outils simples et des prix prévisibles au support conçu pour les entreprises en croissance,
        le cloud de DigitalOcean est conçu pour répondre aux besoins uniques des startups et des PME.
      </p>
    </div>
  </div>
</template>
<script lang="ts">
import {defineComponent} from "vue";

export default defineComponent({
  name: "BuilderWidget"
})
</script>
<style lang="scss">
  .builder{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 20px;
  }
</style>
