<template>
  <h1>{{ fullName }}</h1>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  data() {
    return {
      name: 'Bhayron',
      lastname: 'Klivilan'
    }
  },
  computed: {
    fullName(): string {
      return `${this.name} ${this.lastname}`
    }
  }
})
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
