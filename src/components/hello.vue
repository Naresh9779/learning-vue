<script setup>

// text introplation
const myName='Naresh Thapa'
//attribut Binding

const link='https://random.imagecdn.app/v1/image'

//dynamic binding
const imageINfo={
    src:'https://random.imagecdn.app/v1/image',
    alt:'Random One',
    height:400,
    width:400

}
</script>

<template>
<h1>welcome,{{myName}} To our Page</h1>
<a :href='link'>CLick Here</a>
<img :="imageINfo"/>



</template>




