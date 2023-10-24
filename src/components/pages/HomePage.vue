<template>
  <AppBar />
  <v-container class="w-75 fill-height overflow-auto align-start">
    <v-container class="pa-0">
      <v-row class="my-6 align-center pa-0 ma-0">
        <v-col cols="4" class="pl-4">
          <v-img :width="180" aspect-ratio="16/9" cover src="/logo.png" />
        </v-col>
        <v-col cols="5">
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
            <v-col cols="3" class="pa-0">
              <v-btn icon="mdi-cart" variant="text" />
            </v-col>
          </v-row>
        </v-col>
      </v-row>
      <v-container class="d-flex pa-0 mt-15">
        <p class="text-h3 font-weight-bold me-auto ml-5">Featured Shoes</p>
        <DropdownFilter label="Type" :values="types" />
        <DropdownFilter label="Size" :values="sizes" />
        <DropdownFilter label="Color" :values="colors" />
      </v-container>
      <v-container class="d-flex flex-wrap">
        <ShoeItem />
        <ShoeItem />
        <ShoeItem />
        <ShoeItem />
        <ShoeItem />
        <ShoeItem />
        <ShoeItem />
        <ShoeItem />
        <ShoeItem />
        <ShoeItem />
        <ShoeItem />
      </v-container>
    </v-container>
  </v-container>

  <div class="footer bg-grey-lighten-4 w-100"></div>
</template>

<style scoped>
.footer {
  height: 200px;
}
</style>

<script setup>
import AppBar from "../AppBar.vue";
import DropdownFilter from "../DropdownFilter.vue";
import ShoeItem from "../ShoeItem.vue";

const types = ["sneakers", "boots", "slippers"];
const sizes = ["small", "medium", "large"];
const colors = ["red", "blue", "green"];
</script>
