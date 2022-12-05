<template>
  <div class="container d-flex">
    <img :src="photo" alt="" class="img-fluid r-16">
  </div>
</template>

<script>
export default {
  name: 'AdvertisingComponent',
  props: ['photo']
}
</script>

<style scoped>

</style>
