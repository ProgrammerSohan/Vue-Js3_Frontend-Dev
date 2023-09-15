<template lang="">
    <div>
            <h1>Vue LifeCycle Hooks</h1>
            <ul>
                <li v-for="(item, n) in list" :key="n">

                    {{ item}}
                </li>
            </ul>

    </div>
</template>
<script>
export default {
    data(){
        return {
            list: [
            'Apex Legends',
            'A Plague Tale: Innocence',
            'ART SQOOL',
            'Baba Is You',
            'Devil May Cry 5',
            'The Division 2',
            'Hypnospace Outlay',
            'Katana Zero',
            
            ]

        }
    },
    beforeCreate(){
        alert('beforeCreate: data is static, thats it');
    },
    created(){
        alert('created: data and events ready, but no DOM');
    }

}

</script>