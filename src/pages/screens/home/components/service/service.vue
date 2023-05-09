<template>
  <div class="services">
    <div class="container">
      <div class="services-body">
        <div class="service">
          <div class="service-title">1er</div>
          <div class="subtext-dark">
            Dans la convivialité IaaS, VPS pour les PME et hébergement SMB
          </div>
        </div>
        <div class="service">
          <div class="service-title">15</div>
          <div class="subtext-dark">Centres de données distribués à l'échelle mondiale</div>
        </div>
        <div class="service">
          <div class="service-title">99,99 %</div>
          <div class="subtext-dark">SLA de disponibilité pour le stockage de blocs Droplets et Volumes</div>
        </div>
        <div class="service">
          <div class="service-title">600k</div>
          <div class="subtext-dark">Clients construisant avec DigitalOcean</div>
        </div>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
  import { defineComponent } from "vue";

  export default defineComponent({
    name: 'ServiceComponent'
  })
</script>
<style lang="scss">
  .services{
    border: solid 1px #eaeaea;
    margin-top: 320px;
    margin-bottom: 50px;
    //background: rgba(224, 234, 255, 1);
    .services-body{
      padding: 40px 0;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 50px;
    }
  }
  .service{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 10px;
    padding: 0 33px;
    flex-grow: 1;
    text-align: center;
    border-right: solid 2px #eaeaea;
    .service-title{
      font-size: calc(58px + (60 - 58) * ((100vw - 500px) / (1440 - 320)));
      line-height: 1.14em;
      letter-spacing: -.05em;
      font-weight: 700;
    }
  }
</style>
