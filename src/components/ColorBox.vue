<script setup lang="ts">
</script>

<template>
<div class="square-row">
    <div class="square red"></div>
    <div class="square blue"></div>
    <div class="square green"></div>
  </div>
</template>

<style scoped lang="scss">
.square-row {
  display: flex; /* Sử dụng Flexbox để sắp xếp các phần tử theo hàng ngang */
  justify-content: space-around; /* Khoảng cách đều giữa các phần tử */
}

.square {
  width: 200px;
  height: 200px;
}

.red {
  background-color: red;
}

.green {
  background-color: green;
}

.blue {
  background-color: blue;
}
</style>
