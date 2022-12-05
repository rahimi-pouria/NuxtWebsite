<template>
  <div class="container Footer g24 p-5 d-flex flex-column w-100">
    <div class="d-flex FooterLinks flex-wrap justify-content-between">
      <div class="col-md-2 col-sm-6 LinksResponsive d-flex flex-column g4">
        <h4 class="f18-700 text-right">
          درباره سایت
        </h4>
        <nuxt-link v-for="(item, i) in About" class="text-right" :key="i" to="">
          {{ item }}
        </nuxt-link>
      </div>
      <div class="col-md-2 col-sm-6 LinksResponsive d-flex g4 flex-column">
        <h4 class="f18-700 text-right">
          درباره سایت
        </h4>
        <nuxt-link v-for="(item, i) in About" class="text-right" :key="i" to="">
          {{ item }}
        </nuxt-link>
      </div>
      <div class="col-md-2 col-sm-6 LinksResponsive d-flex g4 flex-column">
        <h4 class="f18-700 text-right">
          درباره سایت
        </h4>
        <nuxt-link v-for="(item, i) in About" class="text-right" :key="i" to="">
          {{ item }}
        </nuxt-link>
      </div>
      <div class="col-md-2 col-sm-6 LinksResponsive d-flex g4 flex-column">
        <h4 class="f18-700 text-right">
          درباره سایت
        </h4>
        <nuxt-link v-for="(item, i) in About" class="text-right" :key="i" to="">
          {{ item }}
        </nuxt-link>
      </div>
      <div class="col-md-2 col-sm-6 LinksResponsive d-flex g4 flex-column">
        <h4 class="f18-700 text-right">
          درباره سایت
        </h4>
        <nuxt-link v-for="(item, i) in About" class="text-right" :key="i" to="">
          {{ item }}
        </nuxt-link>
      </div>
    </div>
    <div class="d-flex flex-wrap justify-content-between">
      <div class="col-md-6 d-flex flex-column g16 text-right p-4">
        <h4 class="f18-700">فروشگاه اینترنتی پاساژ</h4>
        <p class="f14-400">پاساژ یک مرکز خرید و فروش آنلاین کالاست که خدمات خود را به صورت رایگان (بدون کارمزد) ارائه می نماید. هم اکنون بیش از 15,000 فروشگاه از سراسر ایران در حال فعالیت در پاساژ می باشند.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterComponent',
  data () {
    return {
      About: ['درباره سایت', 'معرفی سایت', 'تماس با سایت', 'دانلود اپلیکیشن']
    }
  }
}
</script>

<style scoped lang="scss">
//  responsive
@media only screen and (max-width:600px){
  .Footer{
    padding: 0!important;
  }
  .FooterLinks{
    gap: 15px;
    padding-top: 30px;
  }
  .LinksResponsive{
    width: 48% !important;
  }
}
</style>
