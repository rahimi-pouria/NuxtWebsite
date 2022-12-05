<template>
  <div class="d-flex flex-column w-100 g60 pt-5">
    <HomeCarousel />
    <HomeSpecialProducts />
    <HomeAdvertising :photo="photo1" />
    <HomeAutumnDiscounts />
    <HomeModeling />
    <HomeAdvertising :photo="photo2" />
    <HomeListProduct />
    <HomeTrustBuilding />
  </div>
</template>

<script>
export default {
  name: 'HomeComponent',
  data () {
    return {
      photo1: require('assets/img/ads_img_6383090ae0a9f.jpg'),
      photo2: require('assets/img/prinsly.jpg')
    }
  }
}
</script>

<style scoped>

</style>
