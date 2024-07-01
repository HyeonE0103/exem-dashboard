<template>
  <div class="container">
    <SidebarGnb />
    <div class="content">
      <HeaderGnb></HeaderGnb>
      <router-view></router-view>
    </div>
  </div>
</template>

<script setup lang="ts">
import SidebarGnb from './components/common/SidebarGnb.vue'
import HeaderGnb from './components/common/HeaderGnb.vue'
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  min-width: 1200px;
}

.content {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
