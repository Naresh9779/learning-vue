<script setup>

import {ref} from 'vue';

import cssComponent from './cssComponent.vue'
import htmlComponent from './htmlComponent.vue'
const currentTab=ref('cssComponent');

const tabs={
    cssComponent,
    htmlComponent
}

</script>

<template>
<button @click="currentTab='htmlComponent'">HTML</button>
<button @click="currentTab='cssComponent'">CSS</button>

 <component :is="tabs[currentTab]"/>
</template>