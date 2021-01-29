<template>
  <div class="columns">
    <div class="column">
      <Card
        icon="icon1"
        projectName="Cubicol"
        projectTitle="Education management app for teachers"
        projectDescription="Find financial empowerment with access to quick, affordable microloans."
        projectImage="image1">
      <template v-slot:icon>
        <img src="../assets/images/icon1.png" :alt="icon">
      </template>      
      <template v-slot:image>
          <img src="../assets/images/image1.png" :alt="projectImage">
        </template>
      </Card>
    </div>
    <div class="column">
      <Card
        icon="icon1"
        projectName="Cubicol"
        projectTitle="Education management app for teachers"
        projectDescription="Find financial empowerment with access to quick, affordable microloans."
        projectImage="image1"
        cardColor="#7EA3DB">
        <template v-slot:icon>
          <img src="../assets/images/icon1.png" :alt="icon">
        </template>      
        <template v-slot:image>
          <img src="../assets/images/image1.png" :alt="projectImage">
        </template>
      </Card>
    </div>
    <div class="column">
      <Card
        icon="icon1"
        projectName="Cubicol"
        projectTitle="Education management app for teachers"
        projectDescription="Find financial empowerment with access to quick, affordable microloans."
        projectImage="image1"
        cardColor="#FF9850">
        <template v-slot:icon>
          <img src="../assets/images/icon1.png" :alt="icon">
        </template>         
        <template v-slot:image>
          <img src="../assets/images/image1.png" :alt="projectImage">
        </template>  
      </Card>
    </div>
    <div class="column">
      <Card
        icon="icon1"
        projectName="Cubicol"
        projectTitle="Education management app for teachers"
        projectDescription="Find financial empowerment with access to quick, affordable microloans."
        projectImage="image1"
        cardColor="#14D182">
        <template v-slot:icon>
          <img src="../assets/images/icon1.png" :alt="icon">
        </template>
        <template v-slot:image>
          <img src="../assets/images/image1.png" :alt="projectImage">
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

<style scoped></style>
