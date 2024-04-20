<script setup>

import { reactive,watch,ref } from 'vue';
const state=reactive({userName:'Naresh Thapa',loc:['Canada','india']});

const show=ref(false)
const name=ref('')

watch(()=>state.userName
,(newVal,OldVal)=>{
    console.log('NewVal',newVal);
    console.log('OldVal',OldVal);
  
   
})

</script>

<template>

    <div>
        <h1>{{state.userName}}</h1>
        <h2>{{state.loc[0]}}</h2>
        <h2>{{state.loc[1]}}</h2>
    </div>
    <button @click="show=!show">Change Name</button>
    <br/>
    <br/>
    <form v-if="show">
        <input v-model="name" type="Name" placeholder="Enter New Name">

        <button @click.prevent="state.userName=name, show=!show">Change Name</button>
    

    </form>
    

 

  

</template>