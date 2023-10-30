<template>
  <div>
    <NavBar id="navbar" :title="title" left="返回" @click="test"></NavBar>
    <button @click="btnFun">点击</button>
  </div>
</template>

<script>
import NavBar from './NavBar.vue'
export default {
  components: { NavBar },
  data() {
    return {
      title: '标题',
    }
  },
  methods: {
    btnFun() {
      this.title = '内容'
    },
    test() {
      console.log('test')
    },
  },
}
</script>

<style lang="scss" scoped></style>
