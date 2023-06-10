<!-- we will use this component to add a greeting -->

<template>
    <div>Hello World!</div>
</template>

<!-- NOTE -->
<!-- 
    lets say we move the Welcome to another directory called Home

    so the path would be components/Home/Welcome

    then to auto import this component we need to type <HomeWelcome /> (pascal case) in app.vue file

    we can also use kebab case <home-welcome />

    in this case NUXT we must rename the Welcome.vue to HomeWelcome.vue
 -->