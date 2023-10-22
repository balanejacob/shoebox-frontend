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
        <ShoeImagePreview />
      </v-col>
      <v-col cols="6">
        <ShoeDetails />
        <ShoeOrderForm />
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
import ShoeDetails from "../ShoeDetails.vue";
import ShoeOrderForm from "../ShoeOrderForm.vue";
import ShoeImagePreview from "../ShoeImagePreview.vue";
</script>
