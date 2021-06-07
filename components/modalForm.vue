<template>
  <div class="ModalContainer">
    <button @click="showModal = true"><img src="https://img.icons8.com/metro/26/000000/chat.png"/> <label>Conctactanos</label></button>
    <Modal
      :show="showModal"
      :radius="6"
      @close="showModal = false"
      max="420px"
    >
      <div class="formContainerModal">
            <div class="formDiv">
            <div class="contentForm">
                <h3 class="titleForm"> Vive como si navegaras </h3>
                <div> <input class="inputsForm" placeholder="Nombre completo"/> </div>
                <div> <input class="inputsForm" placeholder="Correo Electronico"/> </div>
                <div> <input class="inputsForm" placeholder="Telefono"/> </div>
                <button class="formbutton">Solicitar información</button>
            </div>
            </div>
        </div>
    </Modal>
  </div>
</template>
<script>
import Modal from 'vue-lightweight-modal'
import FormPrincipal from './formPrincipal.vue'

export default {
  data() {
    return {
      showModal: false,
    }
  },
  components: {
    Modal,
    FormPrincipal,
  },
}
</script>