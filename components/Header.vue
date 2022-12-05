<template>
  <div class="container headerSite d-flex flex-wrap w-100 p-4 align-items-center">
    <div class="col-md-2 col-sm-12 d-flex">
      <NuxtLink to="/">
        <img src="@/assets/img/Digikala-logo.png" alt="" class="img-fluid w-100">
      </NuxtLink>
    </div>
    <div class="col-md-7 col-sm-12">
      <b-form-input class="position-relative pr-4" placeholder="جستجو در میان هزاران محصول..." />
      <BIconSearch
        class="position-absolute"
        style="right: 21px;
        top: 12px;"
      />
    </div>
    <div class="col-md-3 col-sm-12 IconAccount d-flex justify-content-between align-items-center">
      <nuxt-link to="" class="align-items-center" style="color: #000000">
        <BIconChat style="font-size: 20px" />
      </nuxt-link>
      <nuxt-link to="" class="align-items-center" style="color: #000000">
        <BIconHeart style="font-size: 20px" />
      </nuxt-link>
      <nuxt-link to="" class="align-items-center" style="color: #000000">
        <BIconBag style="font-size: 20px" />
      </nuxt-link>
      <div class="d-flex align-items-center">
        <BIconPerson style="font-size: 20px" />
        <NuxtLink to="" class="f12-400" style="color: #000000">
          ورود به حساب کاربری
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script>
import { BIconSearch, BIconChat, BIconHeart, BIconBag, BIconPerson } from 'bootstrap-vue'
export default {
  name: 'HeaderComponent',
  components: { BIconSearch, BIconChat, BIconHeart, BIconBag, BIconPerson }
}
</script>

<style scoped lang="scss">
//  responsive
@media only screen and (max-width:600px){
  .headerSite{
    gap: 15px !important;
    display: flex !important;
    flex-direction: column !important;
  }
}
@media only screen and (min-width:768px) and (max-width: 1024px){
  .IconAccount{
    gap: 11px;
  }
}
@media only screen and (min-width:820px) and (max-width: 1180px){
  .IconAccount{
    gap: 11px;
  }
}
</style>
