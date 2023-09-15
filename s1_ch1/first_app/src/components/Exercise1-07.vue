<template lang="">
    <div>
        <div v-for="(value, key) in information"
         :key="key">
        {{key}}: {{value}}
        </div>
    </div>
</template>
<script setup>
const information = {
    title: "My list component information",
    subtitle: "Vue Js Learning",
    items: ["Looping", "Data", "Methods"],

}

</script>
<style>

</style>