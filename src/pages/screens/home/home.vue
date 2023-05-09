<template>
  <div @scroll="handlerScroll">
    <banner-component />
    <service-component />
    <bg-transition />
    <use-case />
    <bg-transition :close="true" />
    <shop-app />
    <builder-widget />
    <blocks-widget />
    <kuik-product />
    <o-sources />
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
import BannerComponent from "pages/screens/home/components/banner.vue";
import ServiceComponent from "pages/screens/home/components/service/service.vue";
import BgTransition from "components/widget/bgTransition.vue";
import UseCase from "pages/screens/home/components/usecase.vue";
import ShopApp from "pages/screens/home/components/shop.vue";
import BuilderWidget from "pages/screens/home/components/builder.vue";
import BlocksWidget from "pages/screens/home/components/blocks.vue";
import KuikProduct from "pages/screens/home/components/kuikProduct.vue";
import OSources from "pages/screens/home/components/sources.vue";

export default defineComponent({
  name: 'HomeScreen',
  components: {
    OSources,
    KuikProduct,
    BlocksWidget,
    BuilderWidget,
    ShopApp,
    UseCase,
    BgTransition,
    ServiceComponent,
    BannerComponent
  },

  setup(){
    const handlerScroll = (params:any)=>{

      console.log(params)
    }

    return{
      handlerScroll
    }
  }
});
</script>
