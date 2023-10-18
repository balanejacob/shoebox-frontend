<template>
  <div
    class="color-variant mr-2 my-1"
    :style="{ backgroundColor: colorHex }"
  ></div>
</template>

<script setup>
// eslint-disable-next-line no-unused-vars
const props = defineProps({
  colorHex: String,
});
</script>
