<template>
  <div class="container">
    <div class="columns">
      <div class="column is-mobile has-text-centered px-6">
        <p class="has-text-white has-text-weight-bold is-size-4">
          I'm <span class="has-text-lblue">Ernesto</span>, a Lima based User
          Interface & Experience Designer.
        </p>
      </div>
    </div>
    <div class="columns">
      <div class="column is-mobile centered px-3">
        <div class="divider has-background-lblue"></div>
      </div>
    </div>
    <div class="columns">
      <div class="column is-mobile has-text-centered info-div">
        <p class="has-text-customGrey is-size-6">
          Passionate about creating innovative and meaningful digital products
          experiences that connects design with human behaviour.
        </p>
      </div>
    </div>
    <div class="columns py-2">
      <div class="column is-mobile has-text-centered">
        <p class="has-text-customGrey find-text">FIND ME ON</p>
      </div>
    </div>
    <div
      class="columns is-mobile centered has-text-white is-size-6 px-6"
    >
      <div class="column is-narrow px-5" @click="goTo('https://www.linkedin.com/in/ernestoq96/')">
        <p class="pointer">LinkedIn</p>
      </div>
      <div class="column is-narrow px-5" @click="goTo('https://dribbble.com/Ernestoq')">
        <p class="pointer">Dribbble</p>
      </div>
      <div class="column is-narrow px-5" @click="goTo('https://www.behance.net/ErnestoQ')">
        <p class="pointer">Behance</p>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "PersonalInfo",
  setup() {
    return {};
  },
  methods: {
    goTo(url: string) {
      window.open(url);
    },
  },
});
</script>

<style lang="scss" scoped>
.divider {
  width: 32px;
  height: 4px;
  border-radius: 4px;
}
.find-text {
  font-size: 12px;
  font-weight: bold;
  letter-spacing: 0.12rem;
}
.info-div {
  padding-left: 1.5rem;
  padding-right: 1.5rem;
  @include from($tablet) {
    padding-left: 155px;
    padding-right: 155px;
  }  
}
</style>
