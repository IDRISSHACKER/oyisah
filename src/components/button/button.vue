<template>
  <a href="" :class="`btn ${variant}`">
    <img v-if="icon.length" :src="icon" alt="" />
    <div> {{ label }} </div>
  </a>
</template>
<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  props: {
    label: {
      type: String
    },
    variant: {
      type: String,
      default: ()=> ""
    },
    icon: {
      type: String,
      default: ()=> ""
    },
  },
  name: "OButton",
})
</script>
