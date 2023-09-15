<template lang="">
    <div>
       <!--  <h1>{{title.toUpperCase() }}</h1> -->
       <h1>{{ isUppercase ? title.toUpperCase() : title}}</h1>
    </div>
</template>
<script>
export default{
    data(){
        return {
            title: 'This is Second Component!',
            //isUppercase: true,
            isUppercase: false,
        }
    },

}

</script>