<template>
  <div
    class="d-flex flex-wrap"
    style="
    border: 1px solid rgb(209, 209, 209);
    width: 98%;
    margin-right: 15px;
    border-radius: 5px;"
  >
    <div class="col-md-4 p-2">
      <img src="@/assets/img/636b7792122e5.jpg" class="img-fluid w-100" alt="">
    </div>
    <div
      class="col-md-8 d-flex flex-wrap text-right"
      style="border-left: 1px solid #d1d1d1 !important;    border-right: 1px solid #d1d1d1;
"
    >
      <div class="d-flex flex-column w-100 g32">
        <!--          header product-->
        <div class="d-flex justify-content-between w-100" style="border-bottom: 1px solid #d1d1d1">
          <div class="d-flex flex-column g12 w-100 p-3">
            <h2 class="f22-400">
              مانتو یلدایی کرپ الیزه ممتاز مدل یلدایی
            </h2>
            <p class="f14-400">
              کد محصول: 873627
            </p>
          </div>
          <div class="d-flex flex-column w-100 justify-content-end g16 p-4">
            <div class="d-flex w-100 g50 justify-content-end">
              <NuxtLink to="">
                <BIconShare />
              </NuxtLink>
              <NuxtLink to="">
                <BIconHeart />
              </NuxtLink>
            </div>
            <div class="d-flex w-100 justify-content-end g4">
              <nuxt-link v-for="(item , i) in 5" :key="i" to="">
                <BIconStarFill style="color: #ffbf00" />
              </nuxt-link>
            </div>
          </div>
        </div>
        <!--          body-->
        <div class="d-flex flex-column justify-content-between g8">
          <!--   first row       -->
          <div class="d-flex flex-wrap">
            <div class="col-md-6 border-bottom g12">
              <div class="d-flex flex-column w-100 g16">
                <strike>1,318,500</strike>
                <div class="d-flex g8">
                  <h3 style="color: red">
                    791,100
                    تومان
                  </h3>
                  <span
                    class="badge-danger d-flex align-items-center justify-content-center"
                    style="width: 15%; height: 25px; border-radius: 15px;
padding-top: 5px"
                  >40%</span>
                </div>
              </div>
              <div class="d-flex flex-column pt-3 pb-3 g16">
                <span>زمان حدودی ارسال :
                  2 روز                  </span>
                <div class="d-flex g4 align-items-center">
                  <img src="@/assets/img/pasazh-club-coin.png" alt="" style="width: 25px; height: 25px">
                  <p class="f12-400">
                    با خرید این محصول 70 سکه در پاساژ کلاب دریافت می کنید.
                  </p>
                </div>
              </div>
            </div>
            <div class="col-md-6 d-flex g16 flex-column justify-content-end">
              <HomeSeller />
            </div>
          </div>
          <!--  secound row        -->
          <div class="d-flex flex-wrap">
            <div class="col-md-6 border-bottom">
              <HomeColorProduct />
            </div>
            <div class="col-md-6 d-flex justify-content-center w-100">
              <HomeDiscountProduct />
            </div>
          </div>
        </div>
        <div class="d-flex">
          <HomeAddCard />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { BIconHeart, BIconShare, BIconStarFill } from 'bootstrap-vue'
export default {
  name: 'DetailProduct',
  components: { BIconHeart, BIconShare, BIconStarFill },
  layout: 'PublicPage'
}
</script>

<style scoped>

</style>
