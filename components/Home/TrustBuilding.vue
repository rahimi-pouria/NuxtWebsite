<template>
  <div class="container d-flex flex-wrap justify-content-between shadow-sm r-20">
    <div v-for="(item, i) in trust" :key="i" class="d-flex col-md-4 col-sm-6 align-items-center g8 p-3">
      <img :src="item.photo" alt="">
      <p>{{ item.title }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TrustBuilding',
  data () {
    return {
      trust: [
        {
          title: 'تضمین کیفیت',
          photo: require('assets/img/bp-safe.eac77ac.png')
        },
        {
          title: '7 روز ضمانت بازگشت کالا',
          photo: require('assets/img/bp-return.f41d27e.png')
        },
        {
          title: 'تماس مستقیم با فروشنده',
          photo: require('assets/img/bp-seller.c4d68b9.png')
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
