<script setup>
import {ref} from 'vue';
const name=ref('');
const email=ref('');
const password=ref('');




</script>

<template>



    <!-- <button @click="$emit('incrementCounter')" >+</button> -->

    <form @submit.prevent="$emit('userInfo',name,email,password)">
        <input type="name" placeholder="Name"  v-model="name">
        <input type="email" placeholder="Email" v-model="email">
        <input type="password" placeholder="Password" v-model="password">
        <button type="submit">Submit</button>

    </form>
</template>