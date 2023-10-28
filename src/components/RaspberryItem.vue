<template>
  <a href="#" class="container">
    <div class="image">
      <img :src="cartData.imgSrc" alt="img" />
    </div>
    <div class="body">
      <div class="logo"><img :src="cartData.logo" /></div>
      <div class="title">{{ cartData.companyTitle }}</div>
    </div>
    <div class="recommendation">{{ cartData.description }}</div>
  </a>
</template>

<script>
export default {
  name: "RaspberryItem",

  props: {
    cartData: {
      type: Object,
      default: () => ({}),
    },
  },
}
</script>

<style lang="css" scoped>
.image {
  width: 200px;
  height: 200px;
  margin-bottom: 5px;
}
.image img {
  width: 200px;
  height: 200px;
  border-radius: 10px;
  max-width: 100%;
}
.body {
  display: flex;
  gap: 10px;
}
a {
  color: white;
  font-size: 20px;
}
</style>
