<script setup>
import Home from './views/home/index.vue';

const menus = ['Home', 'Blog', 'Works', 'About'];
</script>

<template>
  <div class="main">
    <div class="header">
      <div class="logo">
        <a href="/"></a>
      </div>

      <div class="menus">
        <template v-for="menu in menus">
          <span>{{ menu }}</span>
        </template>
      </div>
    </div>

    <div class="container">
      <Home />
    </div>
  </div>
</template>

<style scoped>
.main {
  width: 100%;
  height: 100%;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 36px;
  height: 60px;
  font-weight: bold;
}

.menus {
  display: flex;
  gap: 16px;
  justify-content: flex-end;
  align-items: center;
}

.container {
  display: inline-flex;
  justify-content: center;
  align-items: center;
  height: calc(100vh - 60px);
}
</style>
