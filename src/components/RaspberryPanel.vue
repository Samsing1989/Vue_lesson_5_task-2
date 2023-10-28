<template>
  <div class="bg">
    <raspberry-item
      v-for="card in cardListData"
      :key="card.id"
      :cart-data="card"
    />
  </div>
</template>

<script>
import RaspberryItem from "./RaspberryItem.vue"
export default {
  components: { RaspberryItem },
  name: "RaspberryPanel",
  props: {
    cardListData: {
      type: Array,
      default: () => [],
    },
  },
}
</script>

<style lang="css" scoped>
.bg {
  background-color: #000;
  padding: 20px;
  align-items: center;
  justify-content: center;
  gap: 30px;
  display: inline-flex;
  border-radius: 10px;
  color: white;
}
</style>
