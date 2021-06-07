<template>
  <div class="carouselBuilding">
    <form-principal/><modal-form/>
    <div>
      <img class="logoTheBoat" src="../static/the_boat_black.png" />
    </div>
    <VueSlickCarousel v-bind="settings1">
      <div><img class="carouselBuildingImg" src="../static/the-boat-fachada_106325301a.jpg" /></div>
      <div><img class="carouselBuildingImg" src="../static/the-boat-fachada_106325301a.jpg" /></div>
      <div><img class="carouselBuildingImg" src="../static/the-boat-fachada_106325301a.jpg" /></div>
    </VueSlickCarousel>
  </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
import FormPrincipal from './formPrincipal.vue'
import ModalForm from './modalForm.vue'

export default {
  components: {
    VueSlickCarousel,
    FormPrincipal,
    ModalForm
  },
  data() {
    return {
      settings1: {
        lazyLoad: "ondemand",
        dots: false,
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
