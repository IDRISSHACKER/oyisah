<template>
  <div class="q-py-xl q-px-md" >
    <div class="text-h5">
      Envoyez-nous un message
    </div>
    <q-form>
      <div class="q-my-md q-mr-md " >
        <q-input rounded outlined
                 placeholder="Entrez votre Nom"
        >
          <template v-slot:prepend>
            <q-icon name="fa-solid fa-user" />
          </template>
        </q-input>
      </div>
      <div class="q-my-md q-mr-md">
        <q-input rounded outlined
                 placeholder="Entrez votre E-mail"
        >
          <template v-slot:prepend>
            <q-icon name="fa-solid fa-envelope" />
          </template>
        </q-input>
      </div>
      <div class="q-my-md q-mr-md">
        <q-input rounded outlined
                 placeholder="Entrez le Sujet"
        >
          <template v-slot:prepend>
            <q-icon name="fa-solid fa-envelope-open-text" />
          </template>
        </q-input>
      </div>
      <div class="q-my-md q-mr-md">
        <q-input rounded outlined
                 type="textarea" placeholder="Ecrivez votre message ici..."
        ></q-input>
      </div>
      <div class="q-my-md q-mr-md">
        <q-btn rounded label="Envoyez" no-caps class="full-width text-white" style="background-color: #250a4c"></q-btn>
      </div>
    </q-form>
  </div>
</template>

<script lang="ts">
  import { defineComponent, ref } from 'vue';

  export default defineComponent({
    name: 'FormContact',
    components: {
    },

    setup(){

      return{
      }
    }
  });
</script>


<style scoped lang="scss">
  .form-contact-input {
    border-radius: 500px!important;
  }
</style>
