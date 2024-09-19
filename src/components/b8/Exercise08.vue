<template>
<div>
    <h2>B8</h2>
    <a @click.stop.prevent="doThat" href="http://www.google.com">Link loi</a> <br> <br>
    <a href=" https://www.google.com">link an duoc</a>    
</div>

</template>

<script setup>
    const doThat =()=>{
        alert("Duong dan khong hop le")
    }
</script>

<style>

</style>