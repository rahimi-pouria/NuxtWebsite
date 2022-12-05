<template>
  <div class="d-flex Discount">
    <div class="container g16 d-flex flex-column align-items-center p-5 r-20" style="background: #c7561a">
      <div class="d-flex flex-column text-center text-white g8">
        <h3 class="f20-400">
          تخفیف های پاییزی
        </h3>
        <p class="f16-400">
          از حراج ها جا نمونی
        </p>
      </div>
      <!--  card product    -->
      <div class="d-flex flex-wrap responsiveProduct" style="height: 200px">
        <div v-for="(item, i) in products" :key="i" class="col-md-3">
          <!-- header card -->
          <div class="d-flex shadow-sm">
            <img :src="item.photo" style="width: 100%; height: 220px" class="img-fluid PhotoProduct" alt="">
          </div>
          <!--     footer card     -->
          <div class="d-flex shadow-sm flex-column bg-white justify-content-between FooterCard p-3">
            <div class="d-flex text-right">
              <p class="f16-400 wordHide">
                {{ item.name }}
              </p>
            </div>
            <div class="d-flex flex-column g4">
              <strike class="f12-400">
                {{ item.Discount }}
              </strike>
              <p class="f14-400">
                {{ item.price }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AutumnDiscounts',
  data () {
    return {
      products: [
        {
          name: 'مانتو یلدایی کرپ الیزه ممتاز مدل یلدایی',
          photo: require('assets/img/636b7792122e5.jpg'),
          price: 791000,
          Discount: 1318000
        },
        {
          name: 'کاپشن مردانه وارداتی اورجینال تک رنگ سبز لجنی سفارش روسیه کلاه خزدار',
          photo: require('assets/img/koat.jpg'),
          price: 1755000,
          Discount: 4500000
        },
        {
          name: 'شلوار ترک اصل بدلیل تک سایز بودن',
          photo: require('assets/img/shalvar.jpg'),
          price: 139000,
          Discount: 348000
        },
        {
          name: 'کرم مرطوب کننده دست و صورت کوکولا 75میل کیفیت عالی',
          photo: require('assets/img/kerem.jpg'),
          price: 34000,
          Discount: 85000
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
  .Discount{
    background: rgba(255,228,228,.3215686275);
    padding-top: 3rem;
    padding-bottom: 8rem;
  }
  .FooterCard{
    min-height: 130px;
    border-bottom-left-radius: 20px;
    border-bottom-right-radius: 20px;
  }
  .PhotoProduct{
    border-top-left-radius: 20px;
    border-top-right-radius: 20px;
  }
//  responsive
  @media only screen and (max-width:600px){
    .Discount {
      padding-bottom: 75rem;
    }
    .responsiveProduct{
      gap: 15px;
    }
  }
  @media only screen and (min-width:768px) and (max-width: 1024px){
    .wordHide{
      overflow: hidden;
      text-overflow: ellipsis;
      white-space: nowrap;
    }
  }
  @media only screen and (min-width:820px) and (max-width: 1180px){
    .wordHide{
      overflow: hidden;
      text-overflow: ellipsis;
      white-space: nowrap;
    }
  }
</style>
