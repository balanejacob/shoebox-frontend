<template>
  <div class="rounded-lg mr-2 color-cell"></div>
</template>

<style scoped>
.color-cell {
  background-color: v-bind(colorHex);
  height: 40px;
  width: 80px;
}
</style>

<script setup>
// eslint-disable-next-line no-unused-vars
const props = defineProps({
  colorHex: String,
  disabled: Boolean,
  selected: Boolean,
});
</script>
