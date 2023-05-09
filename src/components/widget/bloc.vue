<template>
  <div class="bloc">
    <img :src="img" alt="">
    <div class="desc">
      <h4 class="text title4"> {{ title }} </h4>
      <p class="subtext-dark"> {{ content }} </p>
    </div>
  </div>
</template>
<script lang="ts">
import {defineComponent} from "vue";

export default defineComponent({
  name: "BlocWidget",
  props: {
    img: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    content: {
      type: String,
      required: true
    },
  }
})
</script>
<style lang="scss">
.bloc{
  display: flex;
  gap: 30px;
  align-items: center;
  justify-content: center;
  img{
    height: auto;
    width: 80px;
  }
  .desc{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 20px;
  }
}
</style>
