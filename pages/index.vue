<template>
  <div>
    <ul>
      <li class="border-2 " v-for="item in this.foods" key="item.id">
        <FoodItem :name="item.name" :limit="item.limit"></FoodItem>
      </li>
    </ul>
    <button class=" border-blue-400 bg-blue-300 border-2 hover:bg-blue-700 fixed right-5 bottom-5 shadow-xl">レシートのスキャン
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      foods: [
        {name: "卵", limit: "3", id: 1},
        {name: "牛肉", limit: "8", id: 2},
        {name: "玉ねぎ", limit: "9", id: 3},
      ]
    }
  }
}
</script>
