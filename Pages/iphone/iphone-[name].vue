
<template>
    <p> This is the page for iphone {{ name }} </p>
    <p> This is the route {{ route }}</p>
    <p> This is the route params {{ route.params }}</p>
    <p> This is route path {{  route.path }}</p>
</template>

<script setup>
// save to route
const route = useRoute() ;

// replace the dashes in the name
const name = computed(() => {
    return route.params.name.replaceAll("-", " ") ;
});

// head management 

useHead({
    title: `Nuxt3 - iphone ${route.params.name}`,
})

</script>