<template>
  <div class="mx-2" :style="{ width: '150px' }">
    <v-select
      clearable
      :label="label"
      :items="values"
      variant="outlined"
    ></v-select>
  </div>
</template>

<script setup>
defineProps({
  label: String,
  values: Array,
});
</script>
