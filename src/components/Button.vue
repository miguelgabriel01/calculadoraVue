<template>
  <button class="button" :class="{double,triple,operation}" @click="$emit('onClick',label)">
    {{label}}
  </button>
</template>

<script>
export default {
name:'Button',
data() {
  return {
    
  }
},
props:{
  label:{},
  operation:{type: Boolean},
  double: {type:Boolean},
  triple:{type:Boolean}
}
}
</script>

<style>
:root{
  --bg-button: #f0f0f0;
  --border-button:solid 1px #888;
}

.button{
  font-size: 1.4rem;
  background-color: var(--bg-button);
  border:nome;
  border-right: var(--border-button);
  border-bottom: var(--border-button);
  outline: none;
}

.button:active{
  background: #ccc;
}

.button.double{
  grid-column: span 2;
}

.button.triple{
  grid-column: span 3;
}

.button.operation:active{
background: #fa8231cc;
}


</style>