<template>
  <div v-if="!close" class="bg-transit"></div>
  <div v-else class="bg-transit2"></div>
</template>
<script lang="ts">
  import {defineComponent} from "vue";

  export default defineComponent({
    name: "bgTransition",
    props: {
      close: {
        type: Boolean,
        default: false
      }
    }
  })
</script>
<style lang="scss">
.bg-transit{
  background-color: rgb(249, 250, 254);
  background-image: url("https://www.digitalocean.com/_next/static/media/top-wave-blue-6.1b592f40.svg");
  display: flex;
  height: 64px;
  overflow: hidden;
  width: 100%;
  margin-top: 80px;
}
.bg-transit2{
  margin-top: 0px !important;
  @extend  .bg-transit;
  background-image: url("https://www.digitalocean.com/_next/static/media/bottom-wave-blue-6.3261027b.svg");
  margin-bottom: 80px !important;
  transform: rotate(0);
}
</style>
