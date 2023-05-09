<template>
  <div class="ocTitle">
    <div class="container">
        <div class="ocTitleBody">
          <h2 class="title2"> {{ title }} </h2>
          <p class="subtext-dark center"> {{ subTitle }}  </p>
        </div>
    </div>
  </div>
</template>
<script lang="ts">
import {defineComponent} from "vue";

export default defineComponent({
  name: "ocTitle",
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
<style lang="scss">
.ocTitle{
  .ocTitleBody{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 30px;
  }
}
</style>
