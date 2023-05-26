<template>
  <div class="container flex flex-center" style="margin-top: 125px">
    <div class="row items-center q-col-gutter-xl">
      <div class="col-md-6">
        <div class="text-weight-bold text-h5">
          Contact Info
        </div>
        <div class="q-py-md q-pr-md text-justify">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aperiam aspernatur, commodi distinctio dolorum earum est exercitationem ipsa iusto, minima minus obcaecati odio officiis, omnis quae qui repellendus sit tempora vero.
        </div>
        <div class="row q-pt-md">
          <div class="col-md-6">
            <div class="text-subtitle1 text-weight-bold">
              Douala
            </div>
            <div class="q-pt-md row no-wrap q-col-gutter-sm">
              <div ><q-icon name="fa-solid fa-map"></q-icon></div>
              <div>
                Deido 3 boutique residence l'estuaire, Douala, Cameroun
              </div>
            </div>
            <div class="q-pt-md row no-wrap q-col-gutter-sm">
              <div ><q-icon name="fa-solid fa-phone"></q-icon></div>
              <div>
                + 237 692 054 962
              </div>
            </div>
            <div class="q-pt-md row no-wrap q-col-gutter-sm">
              <div ><q-icon name="fa-regular fa-envelope"></q-icon></div>
              <div>
                fodingbrice10@gmail.com
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6 shadow-1 " style="border-radius: 15px">
        <form-contact />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
  import { defineComponent, ref } from 'vue';
  import FormContact from 'pages/screens/contact/components/FormContact.vue'

  export default defineComponent({
    name: 'Contact',
    components: {
      FormContact,
    },

    setup(){

      return{
      }
    }
  });
</script>


<style scoped>

</style>
