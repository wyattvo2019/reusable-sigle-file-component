<template>
  <AirportCards :airports="usAirports" />
  <airport-cards :airports="euAirports" />
</template>

<script>
import { ref } from 'vue'
import AirportCards from '@/components/AirportCards.vue'
import usAirportData from '@/data/us-airports.js'
import euAirportData from '@/data/eu-airports.js'
export default {
  name: 'App',
  components: {
    AirportCards
  },
  setup() {
    const usAirports = ref(usAirportData)
    const euAirports = ref(euAirportData)
    return { usAirports, euAirports}
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
