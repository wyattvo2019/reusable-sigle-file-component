<template>
  <AirportCards />
  <airport-cards />
</template>

<script>
import AirportCards from '@/components/AirportCards.vue'

export default {
  name: 'App',
  components: {
    AirportCards
  }
}
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
