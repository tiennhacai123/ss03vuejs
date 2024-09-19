<template>
<div>
    <h2>B11</h2>
<div :style="{backgroundColor:  bg, height:'50px'}"> <br> <br> <br> <br>
    <button  @click="changeBg('blue')">Change backGround</button>
</div>
</div>

  
</template>

<script setup>
import {ref} from 'vue'
const bg = ref('red')
    const changeBg =(color)=>{
        bg.value = color;
    }
</script>

<style scoped>

</style>