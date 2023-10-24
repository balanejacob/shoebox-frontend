<template>
  <div
    class="rounded-lg mr-2 border d-flex justify-center align-center size-cell"
  >
    <p class="text-caption font-weight-bold">{{ size }}</p>
  </div>
</template>

<style scoped>
.size-cell {
  background-color: #f3f3f3;
  height: 40px;
  width: 80px;
}
</style>

<script setup>
// eslint-disable-next-line no-unused-vars
const props = defineProps({
  size: String,
  available: Boolean,
});
</script>
