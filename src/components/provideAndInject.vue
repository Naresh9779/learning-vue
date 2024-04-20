<script setup>
import {inject} from 'vue'
const studentName=inject('studentName');
const studentAge=inject('studentAge');
const studentLoc=inject('studentLoc');
</script>

<template>

<h1>{{ studentName }}</h1>
<h2>{{ studentAge }}</h2>
<h3>{{ studentLoc }}</h3>

</template>