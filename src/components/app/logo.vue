<template>
  <img v-if="!gray" class="logo" src="~/assets/img/oyisah.png" alt="Oyisah brand" />
  <img v-else class="gray logo" src="https://oyisah.com/favicon.ico" alt="Oyisah brand">
</template>
<script lang="ts">
  import { defineComponent } from "vue";

  export default defineComponent({
    name: "appLogo",
    props: {
      gray: {
        type: Boolean,
        default: false
      }
    }
  })
</script>
<style lang="scss">
  .gray{
    filter: grayscale(1);
    opacity: .4;
  }
</style>
