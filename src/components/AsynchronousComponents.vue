<script setup>
import {ref} from 'vue';
const friends=ref(['Naresh ','Malu','Pankaj']);

</script>

<template>

    <ol>
        <li v-for="(friend,i) in friends" :key="i">
            {{friend}}
        </li>
    </ol>


    </template>