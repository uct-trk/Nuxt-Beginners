<template>
  <div class="container">
    <h3>Burası urunun detail ozeti...</h3>
    <p>Ürün id bilgisi : {{ $route.params.productid }}</p>
    <div class="button-container">
      <nuxt-link to="/products" class="button--green">Geri </nuxt-link>
      <button @click="editProduct">Edit</button>
    </div>
  </div>
</template>

<script>
export default {
  validate(arg) {
    // eslint-disable-next-line no-console
    console.log(arg)
    // return arg.params.productid === '2'
    return /^\d+$/.test(arg.params.productid)
  },
  methods: {
    editProduct() {
      this.$router.push('/products/' + this.$route.params.productid + '/edit')
    },
  },
}
</script>
