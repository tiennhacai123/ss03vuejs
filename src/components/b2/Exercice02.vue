<template>
  <div>
    <h2>B2</h2>
    <p :class="elementClass" :id="elementId">Le Dien Tien</p>
  </div>
</template>

<script setup>
    const elementClass = "cssClass";
    const elementId = "cssId";
</script>

<style scoped>
    .cssClass {
        color: red;
    }
    #cssId {
        background-color: cyan;
        width: 100px;
    }
</style>