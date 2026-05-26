<template>
  <header>
    <div class="headerLeft">
      <h1>{{ title }}</h1>
    </div>

    <div class="headerRight">
      <span v-if="userStore.info">{{ userStore.info.name }}[{{ userStore.info.name }}]</span>
    </div>
  </header>
</template>

<script lang="ts" setup>
import { useUserStore } from '@/store/modules/user'

defineOptions({ name: 'LayoutHeader' })

const title = import.meta.env.VITE_APP_TITLE
const userStore = useUserStore()
</script>

<style scoped lang="less">
header {
  display: flex;
  flex: 0 0 auto;
  align-items: center;
  justify-content: space-between;
  padding: 0 10px;
}
</style>
