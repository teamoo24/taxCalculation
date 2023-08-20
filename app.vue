<template>
  <div>
    <p>原価(¥)：<input type="number" v-model="price"></p>
    <p>税率(%)：<input type="number" v-model="tax"></p>
    <h1>支払額：{{ price+(price*(tax*0.01)) }}(¥)</h1>
  </div>
</template>
<script>
  export default {
    data: () => ({
      price: 1000,
      tax:10
    })
  }
</script>