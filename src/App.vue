<template>
  <Navbar />
  <div>
    <PictureComponent />
    <PersonalInfo />
    <CardsContainer />
    <Footer />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Navbar from './components/Navbar.vue'
import PictureComponent from './components/PictureComponent.vue'
import PersonalInfo from './components/PersonalInfo.vue'
import CardsContainer from './components/CardsContainer.vue'
import Footer from './components/Footer.vue'
import './assets/styles/scss/global.scss'

export default defineComponent({
  name: 'App',
  components: {
    Navbar,
    PictureComponent,
    PersonalInfo,
    CardsContainer,
    Footer
  }
})
</script>

<style>
#app {
  overflow: hidden;
}
</style>