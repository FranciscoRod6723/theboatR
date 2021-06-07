<template>
  <v-container>
        <v-row class="mapTextDiv galleryTextDiv" md="12">
        <div class="galleryText"><h2>Galeria de Fotos</h2></div>
      </v-row>
      <v-row class="imgContarinerGallery" mb="12">
        <v-col>
          <VueSlickCarousel v-bind="settings">
              <div v-for="i in 10" :key="i"><div><img  class="imgGallery" :src=imageText(i) /></div></div>
          </VueSlickCarousel>
        </v-col>
      </v-row>
  </v-container>
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
        dots: false,
        arrow:true,
        fade: false,
        infinite: true,
        speed: 400,
        slidesToShow: 1,
        slidesToScroll: 1,
        autoplay: false,
      },
    }
  },
  methods: {
      imageText(i){
        return 'https://res.cloudinary.com/the-boat-playa-del-carmen/image/upload/f_auto,q_auto/v1614106848/the-boat/room-photos/'+i+'.jpg'
      }
  }
}
</script>