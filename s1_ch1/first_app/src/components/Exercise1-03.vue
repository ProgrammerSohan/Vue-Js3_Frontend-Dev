<template lang="">
    <div>
            <!-- <h1>{{ text }}</h1> -->
            <h1 v-once v-text="text"></h1>
    </div>
</template>
<script setup>
const text = 'Directive text';

</script>
<style>

</style>