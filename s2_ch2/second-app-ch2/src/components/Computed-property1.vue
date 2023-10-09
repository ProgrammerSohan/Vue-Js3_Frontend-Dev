<template lang="">
    <div>
        <br> <br>
       <h1>Combining data props</h1>
        <br>
        <h4>{{formalName}}</h4>
    </div>
</template>
<script>
    export default{
        data(){
            return {
                title: 'Mr.',
                surname: 'Sohanur'

            }

        },
        computed: {
            formalName(){
                return `${this.title} 
                      ${this.surname}`;

            }

        }

    }

</script>
<style scoped>
h1{
    font-weight: bold;
    background-color: yellow;

}
h4{
    font-style: italic;
    font-size: larger;
    border: 2px solid blue;
    text-align: center;
    font-weight: bold;

}
h4:hover{
    color: orange;
    background-color: brown;
}

</style>