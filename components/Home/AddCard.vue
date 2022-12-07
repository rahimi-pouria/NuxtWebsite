<template>
  <div class="d-flex w-100 flex-column g16">
    <div class="d-flex w-50 btns g16">
      <nuxt-link to="" class="btn btn-danger p-2 d-flex align-items-center justify-content-center w-100 f14-400 g8 d-flex">
        <BIconCart />
        افزودن به سبد خرید
      </nuxt-link>
      <nuxt-link to=""
                 class="d-flex justify-content-center align-items-center"
                 style="background: #7065ab; width: 50%; color: #fff; border-radius: 8px">چانه زدن</nuxt-link>
    </div>
    <div class="d-flex align-items-center g16">
      <BIconTruck class="f30-400"/>
      <div class="d-flex flex-column g4">
        <p class="f14-700">ارسال به شهر اهواز : رایگان</p>
        <p class="f14-700">ارسال به کل کشور :
          30,000 تومان</p>
      </div>
    </div>
  </div>
</template>

<script>
import { BIconCart, BIconTruck } from 'bootstrap-vue/src/icons/icons'
export default {
  name: 'AddCard',
  components: { BIconCart, BIconTruck }
}
</script>

<style scoped lang="scss">
@media only screen and (max-width:600px){
  .btns{
    width: 100% !important;
  }
}
</style>
