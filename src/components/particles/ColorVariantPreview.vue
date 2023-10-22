<template>
  <div
    class="mr-2 my-1"
    :style="{
      backgroundColor: colorHex,
      height: '10px',
      width: '10px',
      borderRadius: '50%',
    }"
  ></div>
</template>

<script setup>
// eslint-disable-next-line no-unused-vars
const props = defineProps({
  colorHex: String,
});
</script>
