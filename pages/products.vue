<template>
  <div>
    <search-product />
    <nuxt-child />
  </div>
</template>
<script>
  import SearchProduct from "@/components/SearchProduct"
  export default {
    components : {
      SearchProduct
    },
    layout: "product"
  }
</script>



