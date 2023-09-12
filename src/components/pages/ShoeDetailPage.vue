<template>
    <v-container>
        <v-row>
            <v-col cols="12">
                <h1>Shoe Detail Page</h1>
            </v-col>
        </v-row>
        <nav>
            <ul>
                <li><router-link to="/">Home</router-link></li>
                <li><router-link to="/login">Login</router-link></li>
                <li><router-link to="/register">Register</router-link></li>
                <li><router-link to="/shoe/:id">Shoe Detail</router-link></li>
                <li><router-link to="/profile">Profile</router-link></li>
                <li><router-link to="/cart">Cart</router-link></li>
                <li><router-link to="/checkout">Checkout</router-link></li>
                <li><router-link to="/order/:id">Order Detail</router-link></li>
            </ul>
        </nav>
    </v-container>
    
</template>

<script setup>
    //
</script>