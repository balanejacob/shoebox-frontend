<template>
    <AppBar />

    <v-container class="w-75 fill-height overflow-auto align-start">
        <v-container class="pa-0">
            <v-row class="my-6 align-center pa-0">
                <v-col cols="3">
                    <v-img
                        :width="180"
                        aspect-ratio="16/9"
                        cover
                        src="../../../public/logo.png"
                    />
                </v-col>
                <v-col cols="6">
                    <v-row class="justify-center">
                        <v-btn class="mx-2" variant="text">men</v-btn>
                        <v-btn class="mx-2" variant="text">female</v-btn>
                        <v-btn class="mx-2" variant="text">kids</v-btn>
                    </v-row>
                </v-col>
                <v-col cols="3">
                    <!-- <v-text-field placeholder="Search" variant="solo-filled" class="no-shadow" v-bind:rounded="true"></v-text-field> -->
                </v-col>
            </v-row>
            
        </v-container>
    </v-container>
</template>

<script setup>
    import AppBar from '../AppBar.vue'
</script>