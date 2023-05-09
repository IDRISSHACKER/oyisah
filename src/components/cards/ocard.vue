<template>
  <div class="">
    <div class="shop mt mb">
      <div class="shop-body">
        <div class="desc">
          <h3 class="title3">
            {{ title }}
          </h3>
          <p class="white2 text" style="margin-top: 30px">
            {{ desc }}
          </p>
          <div class="link" style="margin-top: 30px">
            <o-link :label="linkText" />
          </div>
        </div>
        <div class="im">
          <img :src="imgLink" alt="">
        </div>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
import {defineComponent} from "vue";
import OLink from "components/button/link.vue";

export default defineComponent({
  name: "oCard",
  components: {OLink},
  props: {
    title: {
      type: String,
      required: true
    },
    desc: {
      type: String,
      required: true
    },
    linkText: {
      type: String,
      required: true
    },
    imgLink: {
      type: String,
      required: true
    }
  }
})
</script>
<style lang="scss">
.shop{
  border-radius: 15px;
  background: #002C9B;

  .shop-body{
    display: flex;
    justify-content: space-between;
    //align-items: baseline;

    .desc{
      padding: 50px;
      flex-grow: 1;

    }
  }
}

.im{
  width: 100%;
  max-width: 500px;
  display: flex;
  align-items: flex-end;
  justify-content: flex-end;
  img{
    min-width: 100%;
  }
}
</style>
