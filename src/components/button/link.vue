<template>
  <a href="" :class="`btn-link ${variant}`">
    <div> {{ label }} </div>
    <div class="link-icon">
      <q-icon name="fa-solid fa-arrow-right-long"></q-icon>
    </div>
  </a>
</template>
<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  props: {
    label: {
      type: String,
      required: true
    },
    variant: {
      type: String,
      default: ()=> ""
    },
  },
  name: "OLink",
})
</script>

<style lang="scss">
  .dark{
    color: rgb(0, 105, 255) !important;
  }
  .btn-link{
    text-decoration: none;
    color: rgb(255, 255, 255);
    font-size: 18px;
    font-family: "JetBrains Mono", monospace;
    font-weight: 600;
    position: relative;
    transition: all 0.2s ease 0s;
    margin-right: 12px;

    display: flex;
    align-items: flex-start;
    justify-content: flex-start;
    gap: 5px;

    .link-icon{
      transition: margin-left linear 300ms;
    }

    &:hover{
      .link-icon{
        margin-left: 10px !important;
      }
    }
  }
</style>
