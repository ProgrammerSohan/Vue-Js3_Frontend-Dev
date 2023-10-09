<template >
    <input v-model="name">
    <br>
    <div>
            <span>{{error}}</span>
    </div>
</template>
<script>
    export default{
        data(){
            return {
                name: '',

            }
        },
        computed: {
            error(){
                return this.name ? '' : 'Name is required Sohan!'

            }

        }

    }

</script>
<style>
</style>