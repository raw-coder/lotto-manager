<template>
  <modal>
    <div slot="header">
      Number Generator
      <a href="#" class="modal-default-button" @click.prevent="onClose">X</a>
    </div>
    <div slot="body">
      Modal Body
    </div>
    <div slot="footer">
      Modal Footer
    </div>
  </modal>
</template>

<script>
import Modal from './Modal'
export default {
  name: 'GeneratorPopup',
  components: {Modal},
  data () {
    return {

    }
  },
  methods: {
    onClose () {
      this.$emit('close')
    },
  },
}
</script>

<style scoped>

</style>
