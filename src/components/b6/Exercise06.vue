<template>
<div>
    <h2>B6</h2>
    <button @click="handleClick('Rikkei Academy')">Get param</button>    
</div>

</template>

<script setup>
    const handleClick = (message) =>{
        console.log(message);
        
    }
</script>

<style>

</style>