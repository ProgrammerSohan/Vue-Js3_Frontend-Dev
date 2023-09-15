<template lang="">
    <div>
        <h1>Looping through array of objects with v-if conditions</h1>
        <ul>
            <li v-for="(item, n) in interests" :key="n">
                {{item.title}}
                <ol v-if="item.favorites.length>1">
                    <li v-for="(fav, m) in item.favorites" :key="m">
                        {{ fav}}
                    </li>
                </ol>
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
    {
        title: "Cricket",
        favorites:["Sachin","Gayle","Brett Lee"]
    }

 ];

</script>
<style>

</style>