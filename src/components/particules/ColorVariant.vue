<template>
  <div
    class="color-variant mr-2 my-1"
    :style="{ backgroundColor: colorHex }"
  ></div>
</template>

<script setup>
import { defineProps } from "vue";

// eslint-disable-next-line no-unused-vars
const props = defineProps({
  colorHex: String,
});
</script>
