<template>
  <q-layout view="lHh Lpr lFf">
    <q-page-container>
      <header-partial />
      <div>
        <router-view />
      </div>
      <footer-partial />
    </q-page-container>
  </q-layout>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
import HeaderPartial from "layouts/partial/header.vue";
import FooterPartial from "layouts/partial/footer.vue";

export default defineComponent({
  name: 'MainLayout',

  components: {
    FooterPartial,
    HeaderPartial,
  }
});
</script>
