<template>
  <Navbar />
</template>

<script lang="ts">
import { ref, defineComponent } from 'vue'
import Navbar from './Navbar.vue';

export default defineComponent({
  name: 'HelloWorld',
  props: {
    msg: {
      type: String,
      required: true
    }
  },
  components: {
    Navbar
  },
  setup: () => {
    const count = ref(0)
    return { count }
  }
})
</script>

<style scoped>
a {
  color: #42b983;
}
</style>