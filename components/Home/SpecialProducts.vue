<template>
  <div class="container d-flex flex-column justify-content-center g24 w-100">
    <h2 class="f18-700 text-center">
      محصولات ویژه
    </h2>
    <div class="d-flex flex-wrap">
      <div v-for="(item, i) in SpecialProduct" :key="i" class="col-md-2 col-sm-12 g12 d-flex flex-column">
        <img :src="item.photo" alt="">
        <p class="f14-700 text-center">
          {{ item.name }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProductComponent',
  data () {
    return {
      SpecialProduct: [
        {
          name: 'آرایش چشم',
          photo: require('assets/img/a-d-img-63299e9b78bdc.png')
        },
        {
          name: 'آرایش صورت',
          photo: require('assets/img/a-d-img-63299f6d9ae78.png')
        },
        {
          name: 'آرایش لب',
          photo: require('assets/img/a-d-img-63299eebd250e.png')
        },
        {
          name: 'عظر و ادکلن',
          photo: require('assets/img/a-d-img-6329a30fc81bb.png')
        },
        {
          name: 'ضد تعریق ها',
          photo: require('assets/img/a-d-img-63299e9b78bdc.png')
        },
        {
          name: 'مراقبت از پوست',
          photo: require('assets/img/a-d-img-63299f4d225d5.png')
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
