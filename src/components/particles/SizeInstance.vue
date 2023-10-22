<template>
  <div
    class="rounded-lg mr-2 border d-flex justify-center align-center"
    :style="{ backgroundColor: '#F3F3F3', height: '40px', width: '80px' }"
  >
    <p class="text-caption font-weight-bold">{{ size }}</p>
  </div>
</template>

<script setup>
// eslint-disable-next-line no-unused-vars
const props = defineProps({
  size: String,
  available: Boolean,
});
</script>
