<template>
  <div>
    <h2>B12</h2>
    <button @click="changeImage">Change Image</button>
    <div v-if="imageUrl">
      <img :src="imageUrl" alt="Random Image" />
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

// Danh sách các liên kết ảnh
const imageUrls = ref([
  'https://e7.pngegg.com/pngimages/250/129/png-clipart-cat-youtube-humour-blog-russia-cat-mammal-animals.png',
  'https://png.pngtree.com/png-clipart/20240330/ourmid/pngtree-i-m-fine-cat-cute-meme-sticker-png-image_12253789.png',
  'https://play-lh.googleusercontent.com/8ySrSsFPK9pA5vO22g3wPWe-ykWf6LffI_fLQud5OoKrXNljmqJNVaB5MInsQp_twk8',
  'https://lh7-rt.googleusercontent.com/docsz/AD_4nXfVexbOCVCx1E6bGk35u-ztZ_r_cK7YDMiBR46V65_ZoMyEaYDfHED31XPRERi_cD4VsANPqSzjASdN5KiUSFIy23xEzVMYQqqU3sA8QSYlCdQ1HWGpu7llGPk6qCIFa9_QmarHYOTSEPTei9hKbEXBKqQ_?key=v8ba6Z10Wr-7QNx-8gMTgw',
]);

const imageUrl = ref(imageUrls.value[0]);

const changeImage = () => {
  const randomIndex = Math.floor(Math.random() * imageUrls.value.length);
  imageUrl.value = imageUrls.value[randomIndex];
};
</script>

<style scoped>
img {
  width: 400px;
  height: 250px;
}
</style>
