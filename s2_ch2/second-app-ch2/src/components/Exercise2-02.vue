<template lang="">
    <div class="container">
        <h1>Using computed setters</h1>
        <input type="number" v-model="incrementOne">
        <h3>Get input: {{ incrementOne }}</h3>
        <h3>Set division: {{ divideByTwo }}</h3>
    </div>
</template>
<script>
    export default {

        data(){
            return {
                count: -1,
                divideByTwo: 0,
            }
        },
        computed:{
            incrementOne: {
                //getter
                get(){
                    return this.count +1

                },
                //setter
                set(val){

                    this.count = val - 1
                    this.divideByTwo = val /2
                },

            },

        },
       


    }

</script>