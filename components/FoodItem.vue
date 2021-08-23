<template>
  <div class="flex">
    <img class="mr-2"src="/favicon.ico" width="60" height="60"/>
    <div>
      <p>{{ name }}</p>
      <p>賞味期限までおよそあと{{ limit }}日</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "FoodItem",
  props: ['name', 'limit']
}
</script>

<style scoped>

</style>
