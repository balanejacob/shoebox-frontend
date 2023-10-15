<template>
  <div class="shoe-item w-25 d-flex flex-column pa-2 mt-5">
    <div class="shoe-list-image h-100 w-100 bg-grey-lighten-4">
      <v-img src="/src/assets/shoe.png" />
    </div>
    <p class="text-h6 font-weight-bold mt-5 mb-2">Nike Shoe Name 15</p>
    <p class="text-subtitle-2 text-grey-darken-1">Men's Basketball Shoes</p>
    <p class="text-subtitle-2 text-grey-darken-1">US M 7, US M 9</p>
    <div class="d-flex flex-wrap">
      <ColorVariant :color-hex="'#000000'" />
      <ColorVariant :color-hex="'#00FFF0'" />
      <ColorVariant :color-hex="'#FF0000'" />
    </div>
    <p class="text-subtitle-2 text-grey-darken-1">₱ 5,000.00</p>
  </div>
</template>

<script setup>
import ColorVariant from "./particules/ColorVariant.vue";

// eslint-disable-next-line no-unused-vars
const props = {
  colorHex: {
    type: String,
    required: true,
  },
};
</script>
