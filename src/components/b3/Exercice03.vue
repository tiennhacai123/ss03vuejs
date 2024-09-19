<template>
  <div>
      <h2>B3</h2>
       <input v-if="isDisabled" type="text"  disabled > 
       <input v-else placeholder="Cho phep nhap" type="text">
  </div>
</template>

<script setup>
    const isDisabled = true;
</script>

<style>

</style>