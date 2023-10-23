<template>
  <div class="mt-8">
    <p class="text-body-2 font-weight-medium">Color Variations :</p>
    <div class="d-flex mt-2">
      <ColorVariant
        :color-hex="variant"
        v-for="variant in variants"
        :key="variant"
      />
    </div>
  </div>
  <div class="mt-4">
    <p class="text-body-2 font-weight-medium">Sizes :</p>
    <div class="d-flex mt-2">
      <SizeInstance size="M 7" />
      <SizeInstance size="M 8" />
      <SizeInstance size="M 9.5" />
      <SizeInstance size="M 10" />
    </div>
  </div>
  <div class="mt-4">
    <p class="text-body-2 font-weight-medium">Remaining Stocks: 10</p>
  </div>
  <div class="mt-4 d-flex align-center">
    <p class="text-body-2 font-weight-medium">Quantity :</p>
    <div class="d-flex align-center justify-center">
      <v-icon
        size="x-small"
        icon="mdi-minus"
        class="rounded bg-grey-lighten-3 text-grey-darken-1 mx-2"
      />
      <p class="text-body-2 font-weight-medium">1</p>
      <v-icon
        size="x-small"
        icon="mdi-plus"
        class="rounded bg-grey-lighten-2 mx-2"
      />
    </div>
  </div>
</template>

<script setup>
import ColorVariant from "./particles/ColorVariant.vue";
import SizeInstance from "./particles/SizeInstance.vue";

defineProps({
  variants: {
    type: Array,
  },
});
</script>
```
