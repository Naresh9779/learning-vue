<script setup>

import {ref} from 'vue';
const data=ref(null);
const fetchData=()=>{
    fetch('https://jsonplaceholder.typicode.com/todos/1').then((response)=>{

         if(!response.ok)
         {
            throw new Error(`Http Error: ${response.status}`);
         }

         return response.json();



    }).then((responseData)=>{
         data.value=responseData;

    }).catch((error)=>{
        console.log('Error: ${error.message}')
    })

}

</script>

<template>

 

<div>
    <button @click="fetchData">Click To Fetch</button>

    <h1>Fetched Data</h1>
      <div>{{ data }}</div>

</div>


</template>