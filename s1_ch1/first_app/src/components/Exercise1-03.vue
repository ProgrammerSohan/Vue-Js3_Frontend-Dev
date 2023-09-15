<template lang="">
    <div>
            <!-- <h1>{{ text }}</h1> -->
            <h1 v-once v-text="text"></h1>
            <h2 v-html="html"></h2>
    </div>
</template>
<script setup>
const text = 'Directive text';
const html = 'Stylise</br>HTML in<br/><b>your data</b>'

</script>
<style>

</style>