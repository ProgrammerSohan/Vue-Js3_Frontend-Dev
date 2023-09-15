<template lang="">
    <div>
        <h1>Looping through arrays</h1>
        <ul>
            <li v-for="(item, index) in interests"
            :key="index">{{item}}</li>
        </ul>
        <h1> Iterating through an array of objects</h1>
        <ul>
            <li v-for="(item, index) in items" :key="item.id">
                <h2>{{ item.title}}</h2>
                <span>{{item.description}}</span>
               <ul>
                <li v-for="(str, index) in item.characteristics" :key="index">
                    <span>{{str}}</span>
                </li>
               </ul>
            </li>
        </ul>
    </div>
</template>
<script setup>
    const interests = ['TV', 'Games', 'Sports']

    const items = [{
        id: 1,
        title: "Item 1",
        description: "About item 1 Sit molestie sunt, quod? Ullamco ad, hic praesentium hymenaeos commodi corrupti porta animi sapiente? Sunt vitae doloremque, harum nobis itaque illo natoque fuga congue eveniet ultricies assumenda, incididunt! Perferendis.",
        characteristics: ["Summer","Winter","Spring","Autumn"]
    },
    {
        id:2,
        title: "Item 2 ",
        description: "About item 2 Sit molestie sunt, quod? Ullamco ad, hic praesentium hymenaeos commodi corrupti porta animi sapiente? Sunt vitae doloremque, harum nobis itaque illo natoque fuga congue eveniet ultricies assumenda, incididunt! Perferendis.",
        characteristics: ["North", "West", "East", "South"]
    },
    {
        id:3,
        title: 'Item 3',
        description: 'About Item 3 Sit molestie sunt, quod? Ullamco ad, hic praesentium hymenaeos commodi corrupti porta animi sapiente? Sunt vitae doloremque, harum nobis itaque illo natoque fuga congue eveniet ultricies assumenda, incididunt! Perferendis.',
        characteristics: ["Up", "Down", "Left", "Right"]

    }

]

</script>