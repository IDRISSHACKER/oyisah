<template>
<div class="nav">
  <q-header reveal>
    <div class="navbar">
      <div class="brand">
        <app-logo />
      </div>
      <div class="actions">
        <o-button variant="btn-white" label="Connexion" />
        <o-button label="S'inscrire" />
      </div>
    </div>
  </q-header>
</div>
</template>
<script lang="ts">
  import { defineComponent } from "vue";
  import OButton from "components/button/button.vue";
  import AppLogo from "components/app/logo.vue";

  export default defineComponent({
    name: "HeaderPartial",
    components: {AppLogo, OButton},
  })
</script>
<style lang="scss">
  .navbar{
    z-index: 200;
    position: fixed;
    width: 100%;
    padding: 10px 20px;
    background: #ffffff;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  .actions{
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
  }
</style>
