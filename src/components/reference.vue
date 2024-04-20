<script setup>
import {ref,onMounted}from 'vue';
import myEvent from './myEvent.vue';


// const myref = ref('');

// onMounted(()=>{

//    console.log(myref.value);
//    myref.value.focus();
//    myref.value.value='Naresh Thapa';
//    console.log(myref.value.value);
// })

const myref = ref(null);

onMounted(()=>{

    console.log(myref.value);
})
</script>

<template>

<!-- <div>

    <input type="name" placeholder="Enter Your Name" ref="myref" >
</div> -->
<myEvent ref="myref"/>
    
</template>