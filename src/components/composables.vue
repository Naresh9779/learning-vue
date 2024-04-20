<script setup>

import {useCount} from '../composables/useCounter';

const count=useCount();

</script>

<template>

    <h1>Count:{{ count.count }}</h1>
    <button @click="count.increment">Increment</button>
    <button @click="count.decrement">Decrement</button>



</template>