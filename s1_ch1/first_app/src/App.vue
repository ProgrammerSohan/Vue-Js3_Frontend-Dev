<template>
 
    <Exercise />
    <br>
    <Exercise2 />
    <br>
    <Exercise3 />
    <br>
    <h1>V-Model Part</h1>
    <br>
    <Exercise4 />
    <br>
    <h1>Data Iteration with v-for</h1>
    <br>
  <Exercise5 />
  <br>
  <Exercise6 />
  <br>
  <h2> Using v-for to loop through the properties of object</h2>
  <Exercise7 />
  <br>
  <h2>Method Testing</h2>
  <br>
  <MethodExplore />
 
</template>
<script>
import Exercise from './components/Exercise1-01.vue'
import Exercise2 from './components/Exercise1-02.vue'
import Exercise3 from './components/Exercise1-03.vue'
import Exercise4 from './components/Exercise1-04.vue'
import Exercise5 from './components/Exercise1-05.vue'
import Exercise6 from './components/Exercise1-06.vue'
import Exercise7 from './components/Exercise1-07.vue'
import MethodExplore from './components/MethodExplore.vue'
export default {
  components: {
    Exercise,
    Exercise2,
    Exercise3,
    Exercise4,
    Exercise5,
    Exercise6,
    Exercise7,
    MethodExplore

  }

}

</script>
<style> 

</style>