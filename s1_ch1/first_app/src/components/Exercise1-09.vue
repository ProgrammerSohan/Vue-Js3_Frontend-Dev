<template>
    <div>
        <h1>Returning Methods</h1>
        <div>Cart({{ totalItems}}) {{totalCost}}</div>
    </div>
</template>
<script>
 export default {
    data(){
        return {
            totalCost: 0,
            totalItems: 0
        }
        },
        methods: {
            addToCart(n){
                this.totalItems = this.totalItems + 1
                this.totalCost = this.totalCost + n
            }

        }

    

 }

</script>
<style>

</style>