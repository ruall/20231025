<template>
  <div>
    <div>NavBar-{{ title }}-{{ left }}</div>
    <button @click="editTitle">修改标题</button>
    <button v-bind="$attrs">test</button>
    <!-- <NavBarChild></NavBarChild> -->
  </div>
</template>

<script>
import NavBarChild from './NavBarChild.vue'
export default {
  components: [NavBarChild],
  inheritAttrs: false, // 禁止属性透传
  props: ['title', 'left'],
  data() {
    return {}
  },
  methods: {
    editTitle() {
      this.title = '222222'
    },
  },
  computed: {
    title() {
      return this.title + '子组件内容'
    },
  },
}
</script>

<style lang="scss" scoped></style>
