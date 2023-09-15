<template lang="">
    <div>
        <h1>Looping through array of objects with v-if conditions</h1>
        <ul>
            <li v-for="(item, n) in interests" :key="n">
                {{item.title}}
            </li>
        </ul>
    </div>
</template>
<script setup>
 const interests = [
    {
        title: "TV",
        favorites: ["Designed Survivor","Spongebob"],
    },
    {
        title: "Games",
        favorites: ["CS:GO"]
    },
    {
        title: "Sports",
        favorites: [],
    },

 ];

</script>
<style>

</style>