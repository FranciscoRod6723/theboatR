<template>
  <div class="carouselPhrases">
        <div>
          <VueSlickCarousel v-bind="settings">
                <div><h2>No arriesgues tu dinero en inversiones impredecibles como la bolsa</h2></div>
                <div><h2>O en propiedades que aún no están construidas</h2></div>
                <div><h2>Durante 2021 donde te ofrecemos transportación gratuita aeropuerto / condo-hotel / aeropuerto</h2></div>
                <div><h2>Inversión segura con alta plusvalía que podrás disfrutar inmediatamente después de comprar</h2></div>
                <div><h2>Ofrecemos una inversión que podrás gozar de inmediato con tus seres queridos</h2></div>
                <div><h2>Crea nuevas memorias inolvidables mientras tu patrimio cree</h2></div>
            </VueSlickCarousel>
        </div>
  </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'

export default {
  components: {
    VueSlickCarousel,
  },
  data() {
    return {
      settings: {
        lazyLoad: "ondemand",
        dots: true,
        arrows:false,
        fade: false,
        infinite: true,
        speed: 400,
        slidesToShow: 1,
        slidesToScroll: 1,
        autoplay: true,
      },
    }
  },
}
</script>