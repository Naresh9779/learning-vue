
<script setup>

import {ref} from 'vue';

const formData=ref({username:'',email:'',password:''});



</script>
<template>

<form @submit.prevent>

 <input type="name" placeholder="Enter your name" v-model="formData.username">
 <input type="email" placeholder="Enter your email" v-model="formData.email">
 <input type="password" placeholder="Enter your password" v-model="formData.password">
 <button type="sumbit">Sumbit</button>

</form>





<h1>{{ formData.username }}</h1>
<h2>{{ formData.password }}</h2>
<h3>{{ formData.email }}</h3>






</template>