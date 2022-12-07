<template>
  <div class="d-flex flex-column seller">
    <!-- header   -->
    <div class="d-flex w-100 justify-content-between p-2">
      <p class="f14-400 align-items-center pt-1 pr-2">
        فروشنده
      </p>
      <nuxt-link
        to=""
        class="f12-400 d-flex align-items-center btnFoolow justify-content-center"
      >
        دنبال کردن
      </nuxt-link>
    </div>
    <!--  body  -->
    <div class="d-flex p-3 g8">
      <img
        src="@/assets/img/29143_6374fb2ed5981.jpg"
        alt=""
        style="border-radius: 50px; width: 35px; height: 35px"
      >
      <div class="d-flex flex-column g8">
        <p class="f12-400">
          مزون اهواز استایل
        </p>
        <p class="f12-400">طراحی و دوخت انواع مانتو ، عبا ، مچا...</p>
      </div>
    </div>
    <!--    footer -->
    <div class="d-flex w-100">
      <NuxtLink to="" class="p-3 f14-400 w-100 d-flex align-items-center justify-content-center" style="border-left: 1px solid #d1d1d1">تماس با فروشنده</NuxtLink>
      <NuxtLink to="" class="p-3 f14-400 w-100 d-flex align-items-center justify-content-center"> پیام به فروشنده</NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SellerComponent'
}
</script>

<style scoped lang="scss">
  .seller{
    background: #f5f5f5;
    border: solid 1px #e6e6e6;
    border-radius: 8px;
    overflow: hidden;
    min-width: 280px;
  }
  .btnFoolow{
    border: 1px solid #d1d1d1;
    padding: 2px 10px;
    border-radius: 15px;
    height: 25px !important;
  }
</style>
