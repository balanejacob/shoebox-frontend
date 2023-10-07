<template>
  <div class="select mx-2">
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
