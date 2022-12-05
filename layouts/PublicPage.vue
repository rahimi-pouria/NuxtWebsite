<template>
  <div class="d-flex flex-column g8 w-100">
    <div class="d-flex flex-column shadow pb-4">
      <Header />
      <Navbar />
    </div>
    <Nuxt />
    <Footer />
  </div>
</template>

<script>
export default {
  name: 'PublicPage'
}
</script>

<style scoped>

</style>
