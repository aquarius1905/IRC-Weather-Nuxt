<template>
  <div class="home flex">
    <Card v-for="(city, index) in lists" :key="index" :city="city" />
  </div>
</template>

<script lang="ts" setup>
const lists = [
  "sapporo",
  "tokyo",
  "nagoya",
  "osaka",
  "fukuoka",
  "naha"
  ]
</script>

<style scoped>
body {
  background: #eee;
}

.flex {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}
</style>