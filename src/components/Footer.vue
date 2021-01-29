<template>
  <footer class="fs-14">
      <div class="columns">
          <div class="column">
              <p class="has-text-footerText has-text-centered px-4">
                  Yea that’s all for now, more projects coming soon :)
              </p>
          </div>
      </div>
      <div class="columns">
          <div class="column centered">
              <div class="columns has-text-footerText pb-4">
                  <div class="column has-text centered px-5 p-1">Ernesto</div>
                  <div class="column centered px-5 p-0">
                      <div class="divider"></div>
                  </div>
                  <div class="column has-text centered px-5 p-1">Digital Product Designer</div>
              </div>
          </div>
      </div>
      <div class="columns">
          <div class="column centered">
              <div class="columns has-text-footerText pb-4">
                  <div class="column has-text centered px-5 p-1">Social</div>
                  <div class="column centered px-5 p-0">
                      <div class="divider"></div>
                  </div>
                  <div class="column has-text centered px-5 p-1">Linkedin, Instagram, Behance</div>
              </div>
          </div>
      </div>
      <div class="columns pb-6">
          <div class="column centered">
              <div class="columns has-text-footerText pb-">
                  <div class="column has-text centered px-5 p-1">Contact</div>
                  <div class="column centered px-5 p-0">
                      <div class="divider"></div>
                  </div>
                  <div class="column has-text centered px-5 p-1">hola@ernestoq.com</div>
              </div>
          </div>
      </div>
  </footer>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  setup() {
    return {};
  },
});
</script>

<style lang="scss" scoped>
    .divider {
        width: 14px;
        background: $customGrey;
        height: 1px;
    }
</style>
