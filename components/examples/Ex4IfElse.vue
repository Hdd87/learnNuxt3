<template>

<!-- 
  here we create a button when pressed call the function toggle()
  this function change the value of the variable MyComponent to welcome
  when the value of the MyComponent variable is welcome the <HomeWelcome /> component is rendered
  else the <Counter /> component is rendered 
  we use ref to capture changes to the MyComponent variable

-->

<button @click="toggle"> Toggle </button>
    <div v-if="MyComponent === 'welcome'">
        <HomeWelcome />
    </div>
    <Counter v-else />

  
  
</template>


<script setup>

const MyComponent = ref("counter");

function toggle() {
    MyComponent.value = "welcome";
}


</script>
