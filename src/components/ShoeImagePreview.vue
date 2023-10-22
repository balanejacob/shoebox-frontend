<template>
  <div class="bg-grey-lighten-4" :style="{ position: 'relative' }">
    <v-img
      aspect-ratio="16/9"
      cover
      src="/src/assets/shoe.png"
      class="mx-auto"
    />
    <v-img
      aspect-ratio="16/9"
      cover
      src="/src/assets/nike-logo.png"
      class="mx-auto"
      height="100"
      width="100"
      :style="{ position: 'absolute', top: '0', left: '30px' }"
    />
  </div>
</template>

<script setup></script>
