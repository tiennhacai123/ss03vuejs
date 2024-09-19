<template>
  <div>
    <h2>B10</h2>
    <input @input="handleChange" @keydown="handleKeydown" type="text" />
  </div>
</template>

<script setup>
import { ref } from "vue";
const text = ref("");
const handleChange = (event) => {
  text.value = event.target.value;
};
const handleKeydown = (event) => {
  console.log(event);
  if (event.key == "Enter") {
    if (event.shiftKey) {
      alert(text.value);
    } else {
      alert("Bạn cần nhấn Shift + Enter");
    }
  } else {
    return text;
  }
};
// const test1 = ()=>{
//     alert(text.value)
//     text('')
// }
// const test2 = ()=>{
//     alert('Bạn cần nhấn Shift + Enter')
// }
</script>

<style></style>
