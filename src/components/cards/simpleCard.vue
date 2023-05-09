<template>
  <div class="card">
    <div class="card-head">
      <img :src="img" :alt="title">
    </div>
    <div class="card-body">
      <h3 class="title3-card"> {{ title }} </h3>
      <p class="subtext-dark"> {{ content }} </p>
      <o-link variant="dark" label="Apprendre encore plus" style="margin-top: 20px"/>
    </div>
  </div>
</template>
<script lang="ts">
import {defineComponent} from "vue";
import OLink from "components/button/link.vue";
export default defineComponent({
  name: "simpleCard",
  components: {OLink},
  props: {
    img: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      required: true,
    },
    content: {
      type: String,
      required: true,
    },
  }
})
</script>
<style lang="scss">
  .card{
    background-color: rgb(255, 255, 255);
    border-radius: 16px;
    box-shadow: rgba(11, 43, 158, 0.15) 0px 6px 20px -6px;
    display: flex;
    flex-direction: column;
    overflow: hidden;
    text-decoration: none;
    max-width: 400px;

    .card-body{
      display: flex;
      flex-direction: column;
      -webkit-box-flex: 1;
      flex-grow: 1;
      gap: 14px;
      padding: 20px 24px 40px;
    }
  }
</style>
