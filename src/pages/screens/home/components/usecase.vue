<template>
  <div class="usecase">
    <div class="container">
      <div class="usecase-body">
        <h2 class="title2">Comment de vraies entreprises utilisent Oyisah pour accélérer leur croissance</h2>
        <img class="usecase-img" src="https://www.digitalocean.com/_next/static/media/datacake-image.6c12e662.png" alt="">
      </div>
    </div>
  </div>
</template>
<script lang="ts">
import {defineComponent} from "vue";

export default defineComponent({
  name: "useCase"
})
</script>
<style lang="scss">
.usecase{
  background: #e0edff;
  padding-top: 60px;
  padding-bottom: 60px;
  .usecase-body{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 60px;
  }
}
.usecase-img{
  border-radius: 24px;
  max-width: 100%;
}
</style>
