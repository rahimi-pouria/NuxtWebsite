<template>
  <div class="container products-site d-flex flex-wrap">
    <div class="col-md-4">
      <img src="@/assets/img/product.jpg" class="img-fluid w-100" alt="">
    </div>
    <div class="col-md-8 d-flex flex-wrap justify-content-center align-items-center">
      <div
        v-for="(item, i) in products.data"
        :key="i"
        class="col-md-4 g12 align-items-center text-center bg-white"
      >
        <img :src="item.avatar" alt="" class="r-12" style="width: 70%; height: 130px">
        <div class="d-flex g4 pt-3 text-center bg-white
         justify-content-center align-items-center w-100">
          <p class="f14-400 text-center">
            {{ item.first_name }}
          </p>
          <p class="f14-400 text-center">
            {{ item.last_name }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ListProduct',
  data () {
    return {
      products: []
    }
  },
  created () {
    fetch('https://reqres.in/api/users?page=2')
      .then(async (response) => {
        const data = await response.json()
        this.products = data
      })
  }
}
</script>

<style scoped lang="scss">
//  responsive
@media only screen and (max-width:600px){
  .products-site{
    gap: 16px;
  }
}
</style>
