<template>
  <div
    class="rounded-lg mr-2"
    :style="{ backgroundColor: colorHex, height: '40px', width: '80px' }"
  ></div>
</template>

<script setup>
// eslint-disable-next-line no-unused-vars
const props = defineProps({
  colorHex: String,
  disabled: Boolean,
  selected: Boolean,
});
</script>
