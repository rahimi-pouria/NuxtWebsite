<template>
  <div class="d-flex pb-3 w-100  justify-content-center code h-50">
    <div class="d-flex DiscountProduct r-12 flex-column pr-2 pl-2 justify-content-center align-items-center" style="background: #c24545; color: #ffff;border-left: 1px dotted #ffff">
      <p>30%</p>
      <p class="f22-700">Off!</p>
    </div>
    <div class="d-flex align-items-center justify-content-center">
      <div class="d-flex r-12 code flex-column w-100 h-100 g8 justify-content-center align-items-center"
      >
        <p class="f18-400">کد تخفیف: ahvaz</p>
        <span class="f10-400"> تخفیف تا سقف 10000 تومان</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DiscountProduct'
}
</script>

<style scoped lang="scss">
.code{
  padding: 10px 30px !important;
  background: #c24545 !important;
  color: #ffff !important;
}
@media only screen and (max-width:600px){
  .DiscountProduct{
    height: 100% !important;
  }
  //.code {
  //  height: 100% !important;
  //  border-radius: 15px;
  //}
}
</style>
