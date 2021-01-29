<template>
  <div
    :style="'background:' + cardColor"
    class="card-main mx-4 my-3 has-text-centered"
  >
    <!-- <div class="columns py-0 my-0">
      <div class="column">
        <slot name="icon"></slot>
      </div>
    </div> -->
    <div class="columns py-4 my-0">
      <div class="column py-0">
        <h3 class="has-text-white opacity-text">{{ projectName }}</h3>
      </div>
    </div>
    <div class="columns py-0 my-0">
      <div class="column px-6">
        <h1 class="has-text-white has-text-weight-bold">{{ projectTitle }}</h1>
      </div>
    </div>
    <div class="columns py-0 my-0">
      <div class="column py-0">
        <h2 class="has-text-white">{{ projectDescription }}</h2>
      </div>
    </div>
    <div class="columns py-4">
      <div class="column">
        <slot name="image"></slot>
      </div>
    </div>
    <div class="columns py-4 px-5">
      <div class="column">
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
          <div class="column px-5 is-9 has-text-centered">Coming soon</div>
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
}
h2 {
  font-size: 16px;
}
h1 {
  font-size: 24px;
}
.card-main {
  border-radius: 8px;
}
.rounded {
  border-radius: 5px;
}
.opacity-button {
  background-color: transparentize($color: $dark-blue, $amount: .8);
  color: transparentize($color: $dark-blue, $amount: .4);
}
</style>
