<template>
  <div class="input-container">
    <input v-model="productID" type="text" />
    <button class="button--green" @click="showProduct">Ürünü Göster</button>
  </div>
</template>

<script>
export default {
  layout: 'product',
  data() {
    return {
      productID: null,
    }
  },
  methods: {
    showProduct() {
      this.$router.push('/products/' + this.productID)
    },
  },
}
</script>

<style scoped>
.input-container {
  text-align: center;
  padding: 20px;
  border: 1px solid black;
  background-color: #35495e;
}
.button--green {
  border: 1px solid green;
  padding: 10px;
  margin-left: 10px;
  background-color: green;
  color: #dedede;
  text-decoration: none;
  border-radius: 3px;
  cursor: pointer;
}
input {
  border: none;
  outline: none;
  height: 30px;
  font-size: 18px;
  color: #35495e;
}
</style>