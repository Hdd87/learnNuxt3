<template>

  <!-- 
    we use dynamic components using the <component /> tag from vue
    :is syntax is for binding ( see vue )
    the component rendered depends on the value of the varialbe MyComponent
    
    initially we set the value of  MyComponent to Counter component
    the counter component must be resolved using resolveComponent function from Vue
    the shallowRef() is used to capture changes

    when toggle button is pressed, the toggle() function changes the value to HomeWelcome
   -->
  <component :is="MyComponent" />
  <button @click="toggle">Toggle</button>

</template>


<script setup>

const MyComponent = shallowRef(resolveComponent('Counter'));

function toggle() {
  MyComponent.value = resolveComponent('HomeWelcome');
}

</script>
