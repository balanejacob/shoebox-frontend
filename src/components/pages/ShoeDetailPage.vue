<template>
  <v-container class="w-75 fill-height overflow-auto align-start pa-10">
    <div class="d-flex w-100 align-center mt-16">
      <div class="d-flex align-center me-auto">
        <v-icon size="x-large" icon="mdi-keyboard-backspace mr-2" />
        <p class="text-h5 font-weight-bold">Back to Home</p>
      </div>
      <div class="d-flex align-center">
        <p class="text-h6 font-weight-medium mr-2">View Cart</p>
        <v-icon size="large" icon="mdi-cart mr-2" />
      </div>
    </div>
    <v-row class="h-75">
      <v-col cols="6" class="pa-4">
        <div class="bg-grey-lighten-4 shoe-detail-image">
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
            class="mx-auto logo-overlay"
            height="100"
            width="100"
          />
        </div>
      </v-col>
      <v-col cols="6">
        <div class="mt-12">
          <p class="text-h4 font-weight-black">Nike Shoe Name 15</p>
          <p class="text-h5 font-weight-medium text-grey-darken-2 mt-2">
            ₱ 5,000
          </p>
        </div>
        <div class="mt-6">
          <p class="text-body-1 text-grey-darken-1">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat.
          </p>
          <p class="text-body-2 font-weight-bold mt-3">
            Men's Basketball Shoes
          </p>
        </div>
        <div class="mt-8">
          <p class="text-body-2 font-weight-medium">Color Variations :</p>
          <div class="d-flex mt-2">
            <ColorVariant :color-hex="'#000000'" />
            <ColorVariant :color-hex="'#00FFF0'" />
            <ColorVariant :color-hex="'#FF0000'" />
          </div>
        </div>
        <div class="mt-4">
          <p class="text-body-2 font-weight-medium">Sizes :</p>
          <div class="d-flex mt-2">
            <SizeInstance :size="'M 7'" />
            <SizeInstance :size="'M 8'" />
            <SizeInstance :size="'M 9.5'" />
            <SizeInstance :size="'M 10'" />
          </div>
        </div>
        <div class="mt-4">
          <p class="text-body-2 font-weight-medium">Remaining Stocks: 10</p>
        </div>
        <div class="mt-4 d-flex align-center">
          <p class="text-body-2 font-weight-medium">Quantity :</p>
          <div class="d-flex align-center justify-center">
            <v-icon
              size="x-small"
              icon="mdi-minus"
              class="rounded bg-grey-lighten-3 text-grey-darken-1 mx-2"
            />
            <p class="text-body-2 font-weight-medium">1</p>
            <v-icon
              size="x-small"
              icon="mdi-plus"
              class="rounded bg-grey-lighten-2 mx-2"
            />
          </div>
        </div>
        <v-btn
          variant="tonal"
          class="mt-8 w-100 text-subtitle-1 text-capitalize font-weight-bold rounded-0"
          height="60"
          :style="{ backgroundColor: '#ffbd59' }"
        >
          Add to Cart
        </v-btn>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
import ColorVariant from "../particules/ColorVariant.vue";
import SizeInstance from "../particules/SizeInstance.vue";
</script>
