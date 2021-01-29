<template>
  <div class="columns main-container">
    <div class="column child-column">
      <Card
        projectName="Cubicol"
        projectTitle="Education management app for teachers"
        projectDescription="Find financial empowerment with access to quick, affordable microloans."
        isFullProject>
      <template v-slot:image>
          <img src="../assets/images/image1.png" alt="projectImage">
        </template>
      </Card>
    </div>
    <div class="column child-column">
      <Card
        projectName="Cubicol"
        projectTitle="Education management app for teachers"
        projectDescription="Find financial empowerment with access to quick, affordable microloans."
        isFullProject
        cardColor="#7EA3DB">
        <template v-slot:image>
          <img src="../assets/images/image1.png" alt="projectImage">
        </template>
      </Card>
    </div>
    <div class="column child-column">
      <Card
        projectName="Cubicol"
        projectTitle="Education management app for teachers"
        projectDescription="Find financial empowerment with access to quick, affordable microloans."
        isFullProject
        cardColor="#FF9850">    
        <template v-slot:image>
          <img src="../assets/images/image1.png" alt="projectImage">
        </template>  
      </Card>
    </div>
    <div class="column child-column">
      <Card
        projectName="Cubicol"
        projectTitle="Education management app for teachers"
        projectDescription="Find financial empowerment with access to quick, affordable microloans."
        cardColor="#14D182">
        <template v-slot:image>
          <img src="../assets/images/image1.png" alt="projectImage">
        </template>        
      </Card>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Card from "./Card.vue";

export default defineComponent({
  name: "CardsContainer",
  components: {
    Card,
  },
  setup() {
    return {};
  },
});
</script>

<style lang="scss" scoped>
  .main-container {
    @include from($desktop) {
      flex-direction: column;
      align-items: center;
      .child-column {
        max-width: 80vw;
      }
    }
    @include from($tablet) {
      flex-direction: column;
      align-items: center;
    }
  }
</style>
