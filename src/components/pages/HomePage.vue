<template>
  <AppBar />

  <v-container class="w-75 fill-height overflow-auto align-start">
    <v-container class="pa-0">
      <v-row class="my-6 align-center pa-0">
        <v-col cols="3">
          <v-img :width="180" aspect-ratio="16/9" cover src="/logo.png" />
        </v-col>
        <v-col cols="6">
          <v-container>
            <v-row class="justify-center">
              <v-btn class="mx-2" variant="text">men</v-btn>
              <v-btn class="mx-2" variant="text">female</v-btn>
              <v-btn class="mx-2" variant="text">kids</v-btn>
            </v-row>
          </v-container>
        </v-col>
        <v-col cols="3" class="pa-0">
          <v-row class="align-center">
            <v-col cols="9">
              <v-text-field
                label=""
                variant="outlined"
                placeholder="Search"
                hide-details=""
                append-inner-icon="mdi-magnify"
              />
            </v-col>
            <v-col cols="3">
              <v-btn icon="mdi-cart" variant="text" />
            </v-col>
          </v-row>
        </v-col>
      </v-row>
      <v-container class="d-flex pa-0 mt-15">
        <p class="text-h3 font-weight-bold me-auto">Featured Shoes</p>
        <DropdownFilter label="Type" :values="types" />
        <DropdownFilter label="Size" :values="sizes" />
        <DropdownFilter label="Color" :values="colors" />
      </v-container>
    </v-container>
  </v-container>
</template>

<script setup>
import AppBar from "../AppBar.vue";
import DropdownFilter from "../DropdownFilter.vue";

const types = ["sneakers", "boots", "slippers"];
const sizes = ["small", "medium", "large"];
const colors = ["red", "blue", "green"];
</script>
