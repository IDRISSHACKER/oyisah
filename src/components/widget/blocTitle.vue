<template>

</template>
<script lang="ts">
import {defineComponent} from "vue";

export default defineComponent({
  name: "blocTitle",
  props: {
    title: {
      type: String,
      required: true
    },
    subTitle: {
      type: String,
      required: true
    },
  }
})
</script>
