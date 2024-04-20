<script setup>

import {ref,computed} from 'vue';

const number=ref(0)

const Square=computed(()=>number.value**2)

</script>

<template>
<h1>number :{{ number }}</h1>
<h1>square :{{ Square }}</h1>
<button @click="number++">Increase Number</button>

</template>