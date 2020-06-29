<template>
<div>
  Generator
  <button @click.prevent="onClickGenerateButton">Generate!</button>
  <ul>
    <li v-for="number in numbers" :key="number">{{number}}</li>
  </ul>
  <generator-popup
    v-if="isShowingPopup"
    @close="onClosePopup"
  />
</div>
</template>

<script>
import GeneratorPopup from './GeneratorPopup'
export default {
  name: 'Generator',
  components: {GeneratorPopup},
  data () {
    return {
      numbers: () => [1, 2, 3, 4, 5, 6],
      isShowingPopup: false,
    }
  },
  methods: {
    onClickGenerateButton () {
      this.isShowingPopup = true
    },
    onClosePopup () {
      this.isShowingPopup = false
    },
  },
}
</script>

<style scoped>

</style>
