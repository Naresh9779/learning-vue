<script setup>
import {ref} from 'vue';

let count = ref(0);

const incrementHandler=()=>
{
    count.value++;
}

const decrementHandler=()=>
{
    count.value--;
}

const submitHandler=(e)=>{
    e.preventDefault();
    alert('All Things Are Alright');
}
defineExpose({count, incrementHandler, decrementHandler})
</script>

<template>

<h1>My Count :{{ count }}</h1>

<button @click="incrementHandler">Increment</button>
<button @click="decrementHandler">decrement</button>


<!-- <h1 class="head">Fill THis Form</h1>
<form @submit="submitHandler">
    <input type="text" placeholder="Enter Your Name">
    <input type="email" placeholder="Enter Your Email">
    <button type="sumbit">Submit</button>
</form> -->



</template>