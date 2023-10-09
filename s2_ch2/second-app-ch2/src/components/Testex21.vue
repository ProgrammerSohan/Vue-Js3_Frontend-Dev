<template lang="">
    <div>
        <input v-model="firstName" placeholder="first Name">
        <input v-model="lastName" placeholder="last Name">
        <p>{{fullName}}</p>
    </div>
</template>
<script>
export default {
    data(){
        return{
            firstName: '',
            lastName: ''

        }

    },
    computed: {
        fullName(){
            return `${this.firstName} ${this.lastName}`;

        },
    },

}

</script>