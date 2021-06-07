<template>
  <div>
    <div>
      <principal-slider/>
    </div>
    <div>
      <map-container/>
    </div>
    <div>
      <promo-container/>
    </div>
    <div>
      <gallery-container/>
    </div>
    <div>
      <phrases-container/>
    </div>
    <div>
      <inventory-container/>
    </div>
    <div>
      <contact-container/>
    </div>
  </div>
</template>

<script>
import ContactContainer from '../components/contactContainer.vue'
import FormPrincipal from '../components/formPrincipal.vue'
import GalleryContainer from '../components/galleryContainer.vue'
import InventoryContainer from '../components/inventoryContainer.vue'
import MapContainer from '../components/mapContainer.vue'
import PhrasesContainer from '../components/phrasesContainer.vue'
import PrincipalSlider from '../components/principalSlider.vue'
import PromoContainer from '../components/promoContainer.vue'

export default {
  components: {
    PrincipalSlider,
    FormPrincipal,
    MapContainer,
    PhrasesContainer,
    InventoryContainer,
    PromoContainer,
    GalleryContainer,
    ContactContainer
  }
}
</script>