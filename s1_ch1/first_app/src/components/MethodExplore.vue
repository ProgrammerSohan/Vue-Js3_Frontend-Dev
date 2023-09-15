<template lang="">
    <div>
        <button id="click-me" v-on:click="myMethod">Click me</button>
        <button id="click-me" @click="myMethod">Click me shorter</button>
        
    </div>
</template>
<script setup>
const myMethod = () => {console.log('My first method');}

</script>