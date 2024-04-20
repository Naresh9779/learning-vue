<script setup>
import { reactive } from 'vue';

let initialState=reactive({val:{count:0},user:['user1', 'user']})



</script>

<template>

<h1>Count:{{ initialState.val.count }}</h1>
<h1>User:{{ initialState.user }}</h1>
<button @click="initialState.val.count++">+</button>
<button @click="initialState.user.push('thapa')">Add User</button>


</template>