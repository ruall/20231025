<template>
  <div>
    <NavBar @btnFun="testFun"></NavBar>
  </div>
</template>

<script>
import NavBar from './NavBar.vue'
export default {
  components: { NavBar },
  data() {
    return {}
  },
  methods: {
    testFun(data) {
      console.log('abc', data)
    },
  },
}
</script>

<style lang="scss" scoped></style>
