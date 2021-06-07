<template>
  <div class="carouselPromotialPhrases">
        <div>
          <VueSlickCarousel v-bind="settings">
                <div><h2>50% de enganche / 50% financiamiento directo</h2></div>
                <div><h2>3 años sin intereses</h2></div>
                <div><h2>Entrega inmediata </h2></div>
                <div><h2>Desde 147,500 USD*</h2></div>
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