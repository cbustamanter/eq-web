<template>
  <div :style="'background:'+cardColor" class="card-main mx-4 my-6 has-text-centered">
      <div class="columns py-0 my-0">
          <div class="column">
              <img :src="'src/assets/images/'+icon+'.png'" :alt="icon">
          </div>
      </div>
      <div class="columns py-0 my-0">
          <div class="column py-0">
              <h3 class="has-text-white opacity-text">{{projectName}}</h3>
          </div>
      </div>
      <div class="columns py-0 my-0">
          <div class="column px-6">
              <h1 class="has-text-white has-text-weight-bold">{{projectTitle}}</h1>
          </div>
      </div>    
      <div class="columns py-0 my-0">
          <div class="column py-0">
              <h2 class="has-text-white">{{projectDescription}}</h2>
          </div>
      </div>
      <div class="columns py-4">
          <div class="column">
              <img :src="'src/assets/images/'+projectImage+'.png'" :alt="projectImage">
          </div>
      </div>      
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Card",
  props: {
    icon: {
      type: String,
      required: true,
    },
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
    projectImage: {
      type: String,
      required: true,
    },
    cardColor: {
      type: String,
      required: false,
      default: '#2D73EF'
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
</style>
