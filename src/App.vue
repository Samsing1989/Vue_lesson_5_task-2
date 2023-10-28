<template>
  <raspberry-panel :card-list-data="raspberryList" />
</template>

<script>
import RaspberryPanel from "./components/RaspberryPanel.vue"
import { raspberryList } from "./constants/2_data_raspberry"
export default {
  name: "App",
  components: {
    RaspberryPanel,
  },
  data() {
    return {
      raspberryList,
    }
  },
}
</script>

<style>
/* #app {
} */
</style>
