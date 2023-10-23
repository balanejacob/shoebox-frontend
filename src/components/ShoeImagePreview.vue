<template>
  <div class="bg-grey-lighten-4 image">
    <v-img aspect-ratio="16/9" cover :src="image" class="mx-auto" />
    <v-img
      aspect-ratio="16/9"
      cover
      :src="logo"
      class="mx-auto logo"
      height="100"
      width="100"
    />
  </div>
</template>

<style scoped>
.image {
  position: relative;
}
.logo {
  position: absolute;
  top: 0;
  left: 30px;
}
</style>

<script setup>
defineProps({
  image: String,
  logo: String,
});
</script>
