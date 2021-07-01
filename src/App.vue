<template>
  <div id="app">
    <h1>Calculadora</h1>
    <calculator/>
  </div>
</template>

<script>
import Calculator from '../src/main/Calculator.vue'
export default {
  name: 'App',
  components: {Calculator}
}
</script>

<style>

*{
background: ;
}

body{
  margin: 0;
}

#app{
  display: flex;
  flex-direction: column;
  height: 100vh;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: black;
}



</style>
