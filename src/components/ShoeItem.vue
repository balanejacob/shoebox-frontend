<template>
  <div class="shoe-item w-25 d-flex flex-column pa-2 mt-5" @click="showDetails">
    <div class="h-100 w-100 bg-grey-lighten-4 shoe-item">
      <v-img src="/src/assets/shoe.png" />
    </div>
    <p class="text-h6 font-weight-bold mt-5 mb-2">Nike Shoe Name 15</p>
    <p class="text-subtitle-2 text-grey-darken-1">Men's Basketball Shoes</p>
    <p class="text-subtitle-2 text-grey-darken-1">US M 7, US M 9</p>
    <div class="d-flex flex-wrap">
      <ColorVariantPreview color-hex="#000000" />
      <ColorVariantPreview color-hex="#00FFF0" />
      <ColorVariantPreview color-hex="#FF0000" />
    </div>
    <p class="text-subtitle-2 text-grey-darken-1">₱ 5,000.00</p>
  </div>
</template>

<style scoped>
.shoe-item {
  position: relative;
}
</style>

<script setup>
import ColorVariantPreview from "./particles/ColorVariantPreview.vue";

// methods: {
//     showDetails() {
//       this.$router.push(`/shoe/${id}`);
//     }
//   }
</script>
