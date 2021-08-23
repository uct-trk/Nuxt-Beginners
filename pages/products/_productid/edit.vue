<template>
  <div>
    <h3>Burası urunun edit sayfası...</h3>
    <p>Ürün id bilgisi : {{ $route.params.productid }}</p>
    <div class="button-container">
      <nuxt-link
        :to="'/products/' + $route.params.productid"
        class="button--green"
        >Geri
      </nuxt-link>
    </div>
  </div>
</template>

<script>
export default {}
</script>
