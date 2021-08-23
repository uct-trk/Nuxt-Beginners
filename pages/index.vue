<template>
  <section class="container">
    <h1 class="title">Anasayfa</h1>

    <p class="subtitle">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia tenetur
      architecto fugiat laudantium saepe adipisci quaerat laborum. Non ipsam
      tempore quibusdam obcaecati incidunt saepe perferendis veniam aut, enim
      animi. Nostrum.
    </p>
    <div class="button-container">
      <nuxt-link to="/products" class="button--green">Ürünler </nuxt-link>
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style>
.container {
  min-height: 100vh;
  text-align: center;
  margin-top: 50px;
}
.button-container {
  margin-top: 50px;
  border: 1px solid #392;
  background-color: #dedede;
  padding: 10px;
  display: flex;
  justify-content: center;
}
.title {
  font-family: sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}
.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
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
</style>
