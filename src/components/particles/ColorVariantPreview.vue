<template>
  <div class="mr-2 my-1 preview"></div>
</template>

<style scoped>
.preview {
  background-color: v-bind(colorHex);
  height: 10px;
  width: 10px;
  border-radius: 50%;
}
</style>

<script setup>
// eslint-disable-next-line no-unused-vars
const props = defineProps({
  colorHex: String,
});
</script>
