<template>
  <aside>
    <nav>
      <Menu />
    </nav>
  </aside>
</template>

<script lang="ts" setup>
import Menu from '../Menu/index.vue'

defineOptions({ name: 'LayoutSideBar' })
</script>

<style scoped lang="less">
nav {
  height: 100%;
  overflow-y: auto;
  user-select: none;
}
</style>
