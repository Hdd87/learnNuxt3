<!-- 
  this Counter.vue component will increment and decrement a count variable 
  using NUXT's auto import we can place this component inside app.vue for rendering
  we will be using composition API for this ie script setup  
 -->


<template>

  <button @click="increment" >Increment</button>
  <p> {{ count }}</p>
  <button @click="decrement">Decrement</button>

</template>


<script setup>

  const count = ref(0);

  function increment(){
    count.value++
  }
  
  function decrement() {
    count.value--
  }

</script>