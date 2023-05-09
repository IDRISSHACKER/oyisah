<template>
  <div class="banner">
    <div class="banner-content" style='
    background: url("img/banner-bg.svg");
    background-size: cover;
    background-repeat: no-repeat;'>
      <div class="banner-body" style="margin-top: 350px">
        <div class="banner-title">
          <h1 class="title-illus white text-column">
            <span>Hebergement. </span>
            <span>Workspace. </span>
            <span> Ecommerce.</span>
          </h1>
          <p class="text white2 text-column">
            Quelle que soit votre vision
            - une application SaaS, un site Web,
            une boutique de commerce électronique
            - créez-la ici.
          </p>
          <div class="login-options">
            <o-button variant="btn-transparent" label="Connexion par email" />
            <o-button
              variant="btn-white"
              label="Connexion par google"
              icon="https://doimages.nyc3.digitaloceanspaces.com/google-logo.svg"
            />
            <o-button
              variant="btn-white"
              label="Connexion par github"
              icon="https://doimages.nyc3.digitaloceanspaces.com/github-logo.svg"
            />
          </div>
        </div>
        <div class="banner-illus">
          <img src="img/dashboard.svg" alt="">
        </div>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
  import { defineComponent } from "vue";
  import OButton from "components/button/button.vue";
  export default defineComponent({
    name: "bannerComponent",
    components: {OButton}
  })
</script>
<style lang="scss">

  .login-options{
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 20px;
    height: 130px;
  }

  .banner-illus{
    border-radius: 14px;
    margin: auto;
    margin-top: 20px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;

    img{
      box-shadow:
        rgba(0, 12, 121, 0.1) 0 30px 80px,
        rgba(0, 12, 121, 0.1) 0 12px 24px;
    }
  }

  .banner{
    background: #0069FF;
    border-bottom: 1px solid rgb(227, 232, 244);

    .banner-content{
      height: 800px;
      display: flex;
      justify-content: center;

      .banner-body{
        margin-top: 300px;
        display: flex;
        align-items: center;
        justify-content: center;
        max-width: 800px;
        flex-direction: column;
        .banner-title{
          text-align: center;
          *{
            text-align: center;
          }
        }
      }
    }

  }

</style>
