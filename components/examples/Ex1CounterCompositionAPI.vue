<!-- 
  we use Vue3 composition API here   
  therefore we use script setup instead of script 
-->


<template>
  
  <div>Hello World!</div>
 
  <button @click="increment" >Increment</button>
 
  <p> {{ count }}</p>
  
  <button @click="decrement">Decrement</button>

</template>

<!-- create a script section -->


<script setup>

const count = ref(0);
// since we are using "script setup" we can directly write the functions 
function increment(){
  count.value++
}
function decrement() {
  count.value--
}
</script>

