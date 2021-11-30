<template>
  <h1>Stoplight</h1>
  <GoogleMap
  api-key="AIzaSyD2pMQXi-9tZwWDVv0oTGkiRC0R2Se94oE"
  style="width: 100%; height: 500px"
  :center="center"
  :zoom="12"
  >
  
  </GoogleMap>
</template>

<script>
import { defineComponent } from 'vue'
import { GoogleMap,  } from 'vue3-google-map'
// import { Map } from '@/components/Map.vue'

export default defineComponent({
  components: { GoogleMap },
  
  setup() {
    const center = { lat: 39.7392, lng: -104.9903 }

    return { center }
  },
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
