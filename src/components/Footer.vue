<template>
  <footer class="fs-14 pb-4">
    <div class="columns">
      <div class="column">
        <p class="has-text-centered px-4 has-text-footerText">
          That’s all for now, more projects coming soon :)
        </p>
      </div>
    </div>
    <div class="container">
        <div class="columns">
            <FooterItem msg1="Ernesto" msg2="UX & Product Designer" />
            <FooterItem msg1="Social" msg2="Linkedin - Dribbble - Behance" />
            <FooterItem msg1="Contact" msg2="hola@ernestoq.design" />
        </div>
    </div>    
  </footer>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import FooterItem from "./FooterItem.vue";

export default defineComponent({
  name: "Footer",
  components: {
    FooterItem,
  },
  setup() {
    return {};
  },
});
</script>

<style lang="scss" scoped>

</style>
