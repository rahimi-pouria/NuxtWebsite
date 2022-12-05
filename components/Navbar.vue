<template>
  <div class="container-navbar w-100 d-flex justify-content-between align-items-center p-4">
    <div class="ham-btn d-none flex-column g4 pointer" @click="sidebar = !sidebar">
      <div class="line" :class="{'line1':sidebar}" />
      <div class="line" :class="{'line2':sidebar}" />
      <div class="line" :class="{'line3':sidebar}" />
    </div>
    <transition name="nav">
      <div v-if="sidebar" class="nav-items d-none flex-column g60">
        <NuxtLink v-for="(item,index) in menu" :key="index" to="" class="pointer f14-700 c-title">
          {{ item.name }}
        </NuxtLink>
      </div>
    </transition>
    <div class="d-flex g4 align-items-center responsiveMenu">
      <BIconList />
      <nuxt-link to="">
        دسته بندی
      </nuxt-link>
    </div>
    <div v-for="(item, i) in menu" :key="i" class="d-flex g4 align-items-center responsiveMenu">
      <img :src="item.photo" style="width: 20px; height: 20px" alt="">
      <nuxt-link to="">
        {{ item.name }}
      </nuxt-link>
    </div>
  </div>
</template>

<script>
import { BIconList } from 'bootstrap-vue'
export default {
  name: 'NavbarComponent',
  components: { BIconList },
  data () {
    return {
      sidebar: false,
      menu: [
        {
          name: 'کلاب',
          photo: require('assets/img/pasazh-club.2443059.png'),
          path: ''
        },
        {
          name: 'تحفیف',
          photo: require('assets/img/discount.653b6df.png'),
          path: ''
        },
        {
          name: 'مجله',
          photo: require('assets/img/mag.2e461b4.png'),
          path: ''
        },
        {
          name: ' فروشنده شوید',
          photo: require('assets/img/seller.2ecde0d.png'),
          path: ''
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
.line1{
  transform: translate(5px,5px) rotate(45deg);
}
.line2{
  display: none;
}
.line3{
  transform: translate(5px,-3px) rotate(-45deg);
}
.ham-btn{
  z-index: 110;
  width: 24px;
  height: max-content;
}
.line{
  transition: 300ms;
  border-radius: 12px;
  height: 4px;
  width: 100%;
  background-color: $black;
}
.nav-items{
  position: fixed;
  background-color: $navside;
  z-index: 109;
  right: 0px;
  top: 0;
  height: 100%;
  align-items: center;
  padding: 86px 0;
  width: 180px;
}
.nav{
  position: fixed;
  z-index: 108;
  background-color: $navbg;
  height: max-content;
}
.Notification{
  width: 20px;
  height: 20px;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  right: -4px;
  padding-top: 3px;
}
//responsive
@media only screen and (max-width:800px){
  .nav-row{
    display: none !important;
  }
  .ham-btn, .nav-items{
    display: flex !important;
  }
  .MenuResponsive{
    display: none;
  }
  .profilePhoto{
    width: 40px !important;
    height: 40px !important;
  }
  .NotificationReponsive{
    width: 28px !important;
    height: 28px !important;
  }
  .Notification{
    width: 15px;
    height: 15px;
  }
}
@media only screen and (max-width:600px){
  .responsiveMenu{
    display: none !important;
  }
}
</style>
