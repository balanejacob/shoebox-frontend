<template>
  <div
    class="select-cell rounded-lg mr-2 border d-flex justify-center align-center"
    :style="{ backgroundColor: '#F3F3F3' }"
  >
    <p class="text-caption font-weight-bold">{{ size }}</p>
  </div>
</template>

<script setup>
// eslint-disable-next-line no-unused-vars
const props = defineProps({
  size: String,
  isAvailable: Boolean,
});
</script>
