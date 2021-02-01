<template>
    <div class="column centered pt-5">
      <div class="columns">
        <div class="column footer-centered">
          <div
            class="columns footer-item is-multiline has-text-customGrey pb-4"
          >
            <div class="column is-12">
              <div class="columns">
                <div class="column is-narrow has-text-left has-text-centered-mobile p-1">
                  {{ msg1 }}
                </div>
                <div class="column divider-container is-narrow centered p-0">
                  <div class="divider"></div>
                </div>
              </div>
            </div>
            <div class="column is-12 p-1 has-text-centered-mobile has-text-footerText">
              {{ msg2 }}
            </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "FooterItem",
  props: {
    msg1: {
      type: String,
      required: true,
    },
    msg2: {
      type: String,
      required: true,
    },
  },
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
.divider-container {
  align-items: center;
}
.footer-centered {
  @include until($tablet) {
    display: flex !important;
    justify-content: center !important;
  }
}
.footer-item {
  justify-content: center;
  align-items: center;
}
</style>
