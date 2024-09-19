<template>
  <div>
    <h2>B4</h2>
    <div :class="{ active: isActive }" :style="{ backgroundColor: backgroundColor1 }">
      <p>Block</p>
    </div>
  </div>
</template>

<script setup>

const isActive = true;

const backgroundColor1 = 'blue';
</script>

<style scoped>
.active {
  color: #fff;
}

</style>
