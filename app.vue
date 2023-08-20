<template>
  <div>
    <p>原価：<input type="number" v-model="price"></p>
    <p>税率：<input type="number" v-model="tax"></p>
    <h1>支払額：{{ price*tax }}</h1>
  </div>
</template>
<script>
  export default {
    data: () => ({
      price: "",
      tax:""
    })
  }
</script>