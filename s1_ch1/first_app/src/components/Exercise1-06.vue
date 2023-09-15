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
        <h3>Iterating through a keyed collection(object)</h3>
        <ul>
            <li v-for="(value, key, index) in course" :key="key">
                {{index}}. {{key}}: {{value}}
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
 const course = {
    title: "Software Development with Vue",
    description: 'Learn the awesome of Vue',
    lecturer: 'Programmer Sohan'

 }

</script>
<style setup>
h3{
    color:green;
    font-weight: bold;
}

</style>