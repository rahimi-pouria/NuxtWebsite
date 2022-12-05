<template>
  <div class="container d-flex g24 flex-column w-100">
    <div class="d-flex align-items-center justify-content-center">
      <h3 class="f18-700">
        استایل شو
      </h3>
    </div>
    <div class="d-flex flex-wrap align-items-center ShowModeling">
      <div
        v-for="(item, i) in model"
        :key="i"
        class="col-md-2 col-sm-6 g16 d-flex flex-column
         justify-content-center align-items-center ModelingResponsive"
      >
        <img :src="item.photo" style="width: 100px; height: 100px" alt="">
        <p class="f16-700">
          {{ item.name }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ModelingComponent',
  data () {
    return {
      model: [
        {
          name: 'استایل دانشجویی',
          photo: require('assets/img/studeent.png')
        },
        {
          name: 'استایل مینیمال',
          photo: require('assets/img/minimal.png')
        },
        {
          name: 'استایل کلاسیک',
          photo: require('assets/img/classic.png')
        },
        {
          name: 'استایل اسپرت',
          photo: require('assets/img/sport.png')
        },
        {
          name: 'استایل کژوال',
          photo: require('assets/img/kazhval.png')
        },
        {
          name: 'ترندها',
          photo: require('assets/img/terands.png')
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
//  responsive
@media only screen and (max-width:600px) {
  .ShowModeling {
    gap: 15px;
  }
  .ModelingResponsive{
    width: 47% !important;
  }
}
</style>
