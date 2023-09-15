<template lang="">
    <div>
            <!-- <h1>{{ text }}</h1> -->
            <h1 v-once v-text="text"></h1>
            <h2 v-html="html"></h2>
            <a 
                :href="link.url"
                :target="link.target"
                :tabindex="link.tabindex"

            >{{link.title}}</a>
    </div>
</template>
<script setup>
const text = 'Directive text';
const html = 'Stylise</br>HTML in<br/><b>your data</b>';
const link = {
    title: "Go to Youtube",
    url: 'https://youtube.com',
    tabindex: 1,
    target: '_blank',

};

</script>
<style>

</style>