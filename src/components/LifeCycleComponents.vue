<script setup>
import {ref,onBeforeMount,onMounted,onBeforeUpdate,onUpdated,onBeforeUnmount,onUnmounted} from 'vue'
const message=ref('Hello ,Naresh Thapa');
onBeforeMount(()=>{
console.log('component Is About to Mount')
})
onMounted(()=>{
    console.log('components mounted');
})

onBeforeUpdate(()=>{

    console.log('component Is About to Update');
})


onUpdated(()=>{
    console.log('component Updated');
})

onBeforeUnmount(()=>{
    console.log('component Is About to Unmount');
})

onUnmounted(()=>{
    console.log('component Unmounted');
})


const messageUpdater=()=>{
    message.value='Hello, Pankaj ';
}
</script>

<template>
    
    <h1 >{{ message }}</h1>
    <button @click="messageUpdater">Update Message</button>
</template>