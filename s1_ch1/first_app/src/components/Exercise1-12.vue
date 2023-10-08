<template>
    <div>
        <h1>CSS Modules</h1>
        <h2 :class="$style.title">{{title}}</h2>
        <h3 :class="$style.subtitle">{{subtitle}}</h3>
        <span :class="$style.coder">{{ coder }}</span>

    </div>
</template>
<script>
    export default{
        data(){
            return{
                title: 'CSS module component!',
                subtitle: 'The fourth exercise',
                coder: 'Programmer Sohan'

            }
        },

    }

</script>

<style module>
    h2,h3{
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        text-align: center;
    }
  .title{
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    color: #2c3e50;
    margin-top:60px;
    background-color: yellow;

  }
  .subtitle{
    color: #4fc08d;
    font-style: italic;

  }
  .coder{
    text-align: center;
    border:3px solid blue;
    padding: 5px;
    font-size: 50px;
    font-weight: bolder;

  }

</style>