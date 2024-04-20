<script setup>
import {ref} from 'vue';
const isloggedIn=ref('true')

</script>

<template>

    <div v-show="isloggedIn">
    
        <h1> welcome To page</h1>
        <h2>Welcome To New World</h2>
        <button @click="isloggedIn=!isloggedIn">Logout</button>
    
    
    
    </div>
      <div v-if="!isloggedIn">
    <h1>Tap To Login</h1>
    <button @click="isloggedIn=true">Login Now</button>
    </div>

    <!-- We Also Have v-else-if && v-else -->


</template>