<template>
  <div
    :style="'background:' + cardColor"
    class="card-main mx-4 my-3 has-text-centered-mobile"
  >
    <div class="columns py-4 my-0">
      <div class="column centered-container is-6">
        <div class="columns is-multiline">
          <div class="column is-10 is-offset-2 pl-0-tablet">
            <h3 class="has-text-white opacity-text">{{ projectName }}</h3>
          </div>
          <div class="column is-10 is-offset-2 pl-0-tablet">
            <h1 class="has-text-white has-text-weight-bold">
              {{ projectTitle }}
            </h1>
          </div>
          <div class="column is-10 is-offset-2 pl-0-tablet">
            <h2 class="has-text-white">{{ projectDescription }}</h2>
          </div>
          <div class="column btn1 is-4-fullhd is-offset-2 is-6-tablet">
            <div
              class="columns rounded has-background-dark-blue is-mobile has-text-white has-text-weight-bold"
              v-if="isFullProject"
            >
              <div class="column px-5 has-text-left is-9">Full Project</div>
              <div class="column">
                <img src="../assets/svg/arrow.svg" />
              </div>
            </div>
            <div
              class="columns rounded opacity-button has-text-weight-bold"
              v-else
            >
              <div class="column px-5 has-text-centered">Coming soon</div>
            </div>
          </div>
        </div>
      </div>
      <div class="column centered-container is-6">
        <div class="columns">
          <div
            class="column px-0 is-offset-5-widescreen is-6-widescreen is-offset-4 is-7 is-offset-1-mobile is-10-mobile"
          >
            <slot name="image"></slot>
          </div>
        </div>
      </div>
      <div class="column btn2 is-4-fullhd is-offset-2 is-offset-1-mobile is-10-mobile">
        <div
          class="columns rounded has-background-dark-blue is-mobile has-text-white has-text-weight-bold"
          v-if="isFullProject"
        >
          <div class="column px-5 has-text-left is-9">Full Project</div>
          <div class="column">
            <img src="../assets/svg/arrow.svg" />
          </div>
        </div>
        <div class="columns rounded opacity-button has-text-weight-bold" v-else>
          <div class="column px-5 has-text-centered">Coming soon</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Card",
  props: {
    projectName: {
      type: String,
      required: true,
    },
    projectTitle: {
      type: String,
      required: true,
    },
    projectDescription: {
      type: String,
      required: true,
    },
    cardColor: {
      type: String,
      required: false,
      default: "#2D73EF",
    },
    isFullProject: {
      type: Boolean,
      required: false,
      default: false,
    },
  },
  setup() {
    return {};
  },
});
</script>

<style lang="scss" scoped>
.opacity-text {
  font-weight: 500;
  opacity: 0.7;
}
h3 {
  font-size: 18px;
  @include from($desktop) {
    font-size: 16px;
  }
}
h2 {
  font-size: 16px;
  @include from($desktop) {
    font-size: 16px;
  }
}
h1 {
  font-size: 24px;
  @include from($desktop) {
    font-size: 28px;
  }
}
.btn2 {
  @include until($tablet) {
    display: block;
  }
}
.btn1 {
  @include until($tablet) {
    display: none !important;
  }
}
.card-main {
  border-radius: 8px;
}
.rounded {
  border-radius: 5px;
}
.opacity-button {
  background-color: transparentize($color: $dark-blue, $amount: 0.8);
  color: transparentize($color: $dark-blue, $amount: 0.4);
}
.centered-container {
  @include from($desktop) {
    display: flex;
    align-items: center;
  }
}
</style>
