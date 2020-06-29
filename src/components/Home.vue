<template>
  <div>
    <generator></generator>
    <hr/>
    <number-list></number-list>
  </div>
</template>

<script>
import Generator from './Generator'
import NumberList from './NumberList'
export default {
  name: 'Home',
  components: {
    NumberList, Generator,
  },
}
</script>

<style scoped>

</style>
