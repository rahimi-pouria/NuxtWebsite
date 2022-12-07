<template>
  <div class="d-flex flex-column g16 pb-3">
    <div class="d-flex align-items-center g8">
      <p class="f12-400">
        رنگ :
      </p>
      <span
        class="d-flex justify-content-between align-items-center g8"
        style="border: solid 2px #18d2c7; padding: 5px 10px; border-radius: 17px"
      >
        <span class="rounded-circle bg-danger" style="width: 20px; height: 20px" />
        <p>زرشکی</p>
      </span>
    </div>
    <div class="d-flex g8">
      <p class="f12-400">
        سایز:
      </p>
      <div class="d-flex w-100 flex-wrap justify-content-between g8">
        <span
          v-for="(item, i) in size"
          :key="i"
          class="size f14-400 d-flex text-center justify-content-between align-items-center g8"
        >{{ item }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ColorProduct',
  data () {
    return {
      size: ['x-34', 's-36',
        'M-38', 'L-40', 'Xl-42', '2XL-44', '3Xl-46', '4Xl-48',
        '5Xl-50', '6Xl-52', '8Xl-54', '10Xl-56', '3Xl-46', '12Xl-58', '14Xl-60', 'free size']
    }
  }
}
</script>

<style scoped lang="scss">
  .size{
    border: solid 2px #d1d1d1;
    width: 20%;
    height: 30px;
    text-align: center;
    padding-right: 8px;
    padding-left: 8px;
    border-radius: 17px;
    justify-content: center !important;
    align-items: center !important;
    padding-top: 4px;
  }
</style>
