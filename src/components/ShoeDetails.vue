<template>
  <div class="mt-12">
    <p class="text-h4 font-weight-black">{{ name }}</p>
    <p class="text-h5 font-weight-medium text-grey-darken-2 mt-2">
      ₱ {{ price }}
    </p>
  </div>
  <div class="mt-6">
    <p class="text-body-1 text-grey-darken-1">
      {{ description }}
    </p>
    <p class="text-body-2 font-weight-bold mt-3">{{ type }}</p>
  </div>
</template>

<script setup>
defineProps({
  name: String,
  price: Number,
  description: String,
  type: String,
});
</script>
