<template>
  <div></div>
</template>

<script>
export default {
  name: 'NumberList',
  props: {
    num: {
      type: Object,
      nullable: true,
      default: () => [ 1, 2, 3, 4, 5, 6 ],
    },
  },
}
</script>

<style scoped>

</style>
