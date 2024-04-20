<script setup>

import {ref} from 'vue';

// const detail=defineProps(['firstName', 'lastName'])
// props are immutable only read only

// const details=defineProps({data:Object})
    
// custom Validator

const data=defineProps({name:{
    type:String,
    validator:(propValue)=>{
        return ['Malu','Vinay','Naresh'].includes(propValue);
    }
}})

</script>

<template>


<!-- <h1>{{ details}}</h1> -->
<hr />

<!-- <ul v-for="(item,i) in details" :key="i">{{ item }}

        <li v-for="(it,i) in item " :key="i">{{ it }}</li>
             <li v-for="(itm,i) in it" :key="i">{{ itm }}</li>


</ul>
     -->
     <h1>{{ name}}</h1>






</template>