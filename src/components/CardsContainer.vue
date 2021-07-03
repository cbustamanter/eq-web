<template>
  <div class="columns main-container">
    <div class="column child-column">
      <Card
        projectName="CUBICOL"
        projectTitle="Diseñando la experiencia de una app móvil para colegios"
        projectDescription="Cubicol es una aplicación móvil que busca minimizar el esfuerzo que los padres realizan para enterarse de la vida escolar de sus hijos."
        projectUrl="https://www.figma.com/proto/g8ZPaojhD2QHD3Rd6Gy7WCsN/EQ-Portafolio-2021?page-id=0%3A1&node-id=513%3A79&viewport=5900%2C265%2C0.38463565707206726&scaling=scale-down-width"
        isFullProject>
      <template v-slot:image>
          <img src="../assets/images/home-cubicol.png" alt="projectImage">
        </template>
      </Card>
    </div>

    <div class="column child-column">
      <Card
        projectName="CULQI"
        projectTitle="Plataforma omnicanal para la trazabilidad de pagos en línea"
        projectDescription="El panel de Culqi permite a sus clientes gestionar desde un solo lugar todas sus transacciones realizadas a través del checkout integrado a su plataforma."
        projectUrl="https://www.figma.com/proto/g8ZPaojhD2QHD3Rd6Gy7WCsN/EQ-Portafolio-2021?page-id=848%3A1&node-id=848%3A7926&viewport=507%2C349%2C0.13285091519355774&scaling=scale-down-width"
        isFullProject
        cardColor="#10C58F">
        <template v-slot:image>
          <img src="../assets/images/home-culqi.png" alt="projectImage">
        </template>
      </Card>
    </div>

    <div class="column child-column">
      <Card
        projectName="DUUVI"
        projectTitle="Plataforma digital para gestores de eventos"
        projectDescription="Duuvi permite gestionar eventos y ponerlos a disposición de las personas que busquen cualquier tipo de entretenimiento, ya sea presencial o en línea." 
        projectUrl="https://www.figma.com/proto/g8ZPaojhD2QHD3Rd6Gy7WCsN/EQ-Portafolio-2021?page-id=784%3A5&node-id=784%3A6&viewport=484%2C335%2C0.05643229931592941&scaling=scale-down-width"
        isFullProject     
        cardColor="#7EA3DB">
        <template v-slot:image>
          <img src="../assets/images/home-duuvi.png" alt="projectImage">
        </template>
      </Card>
    </div>    

    <div class="column child-column">
      <Card
        projectName="ENVAIRY"
        projectTitle="Cómo medir el clima laboral de toda una organización"
        projectDescription="Envairy permite realizar mediciones de clima laboral y obtener resultados en tiempo real, asimismo facilita a los líderes diseñar estrategias para mejorar."
        projectUrl="https://www.figma.com/proto/g8ZPaojhD2QHD3Rd6Gy7WCsN/EQ---Portafolio---2021?node-id=513%3A79&scaling=min-zoom"
        cardColor="#F9934C">
        <template v-slot:image>
          <img src="../assets/images/home-envairy.png" alt="projectImage">
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
        max-width: 1050px;
      }
    }
    @include from($tablet) {
      flex-direction: column;
      align-items: center;
    }
  }
</style>
