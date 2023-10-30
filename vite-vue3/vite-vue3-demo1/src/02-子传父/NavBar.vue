<template>
  <div>
    <div>NavBar</div>
    <button @click="clickFun">子组件传值</button>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
  methods: {
    clickFun() {
      this.$emit('btnFun', 'test')
    },
  },
}
</script>

<style lang="scss" scoped></style>
