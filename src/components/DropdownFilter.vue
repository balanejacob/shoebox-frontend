<template>
  <div class="mx-2 filter">
    <v-select
      clearable
      :label="label"
      :items="values"
      variant="outlined"
    ></v-select>
  </div>
</template>

<style scoped>
.filter {
  width: 150px;
}
</style>

<script setup>
defineProps({
  label: String,
  values: Array,
});
</script>
