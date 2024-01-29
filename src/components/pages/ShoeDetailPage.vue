<template>
  <v-container class="w-75 fill-height overflow-auto align-start pa-10">
    <div class="d-flex w-100 align-center mt-16">
      <div class="d-flex align-center me-auto">
        <v-icon size="x-large" icon="mdi-keyboard-backspace mr-2" />
        <router-link to="/" class="text-h5 font-weight-bold">
          Back to Home
        </router-link>
      </div>
      <div class="d-flex align-center">
        <p class="text-h6 font-weight-medium mr-2">View Cart</p>
        <v-icon size="large" icon="mdi-cart mr-2" />
      </div>
    </div>
    <v-row class="h-75">
      <v-col cols="6" class="pa-4">
        <ShoeImagePreview
          image="/src/assets/shoe.png"
          logo="/src/assets/nike-logo.png"
        />
      </v-col>
      <v-col cols="6">
        <ShoeDetails
          name="Nike Shoe Name 15"
          price="5000"
          description="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod 
          tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
          veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
          commodo consequat."
          type="Men's Basketball Shoes"
        />
        <ShoeOrderForm :variants="colors" />
        <v-btn
          variant="tonal"
          class="button-color mt-8 w-100 text-subtitle-1 text-capitalize font-weight-bold rounded-0"
          height="60"
        >
          Add to Cart
        </v-btn>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
.button-color {
  background-color: #ffbd59;
}
</style>

<script setup>
import ShoeDetails from "../ShoeDetails.vue";
import ShoeOrderForm from "../ShoeOrderForm.vue";
import ShoeImagePreview from "../ShoeImagePreview.vue";

const colors = ["#000000", "#00FFF0", "#FF0000"];
</script>
