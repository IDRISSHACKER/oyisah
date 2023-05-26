<template>
  <div>
    <div class="footer">
      <div class="container">
        <div class="footer-body">
          <div class="brand copy-val">
            <app-logo :gray="true" />
            <div class="copy">© 2023 Oyisah, LLC. All rights reserved.</div>
          </div>
          <div class="links">
            <div class="policy">

            </div>
            <ul class="socials">
              <li>
                <a href="https://www.facebook.com/profile.php?id=100091885388505&mibextid=ZbWKwL">
                  <q-icon name="fa-brands fa-square-facebook"></q-icon>
                </a>
              </li>
              <li>
                <a href="https://twitter.com/oyisah_?t=E13cmvMM-2EcWpeNZGDbuA&s=09">
                  <q-icon name="fa-brands fa-square-twitter"></q-icon>
                </a>
              </li>
              <li>
                <a href="https://instagram.com/oyisah?igshid=ZDdkNTZiNTM=">
                  <q-icon name="fa-brands fa-square-instagram"></q-icon>
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import OButton from "components/button/button.vue";
import AppLogo from "components/app/logo.vue";

export default defineComponent({
  name: "FooterPartial",
  components: {AppLogo, OButton},
})
</script>
<style lang="scss">
.copy-val{
  display: flex;
  gap: 5px;
  align-items: center;
  font-weight: 600;
  color: #4d5b7c;
}

  .footer{
    padding-top: 50px;
    padding-bottom: 50px;
    .footer-body{
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
  }
  .copy{

  }
  .socials{
    display: flex;
    align-items: center;
    gap: 10px;
    li{
      a{
        font-size: 2.2rem;
        text-decoration: none;
        color: $primary;
      }
    }
  }
</style>
