<script setup></script>

<template>
  <div class="home">
    <div class="left"></div>
    <div class="right">
      <img src="../../assets/me.png" alt="" />
    </div>
  </div>
</template>

<style scoped>
.home {
  display: flex;
  justify-content: space-between;
  margin: 0 auto;
  max-width: 1200px;
}

.left,
.right {
  width: 50%;
}

img {
  width: 100%;
}
</style>
