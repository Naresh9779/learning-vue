<script setup>
import { ref ,reactive} from 'vue';

let userDetails=ref({name:'thapa',email:'thapa@gmail.com',student:'false'})

let friends=reactive([ref('thapa'),ref('malu'),ref('aunty')]);
</script>

<template>
<h1>Name:{{ userDetails.name }}</h1>
<h2>Email:{{ userDetails.email }}</h2>
<h3>Student:{{ userDetails.student }}</h3>

<button @click="userDetails.student=true">Change Student</button>

<h1>1.{{ friends[0] }}</h1>
<h2>2.{{ friends[1] }}</h2>
<h1>3.{{ friends[2] }}</h1>

<button @click="friends[0]='❤️'">HandShake</button>




</template>