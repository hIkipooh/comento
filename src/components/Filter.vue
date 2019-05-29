<template>
  <div>
  <b-button v-b-modal.modal-center>Launch centered modal</b-button>

  <b-modal id="modal-center" centered title="BootstrapVue">
    <p class="my-4">Vertically centered modal!</p>
  </b-modal>
</div>
</template>

<script>
import { ModalPlugin } from "bootstrap-vue/es/components";
import { BModal } from "bootstrap-vue/es/components";

export default {
  data() {}
};
</script>


<style>
</style>