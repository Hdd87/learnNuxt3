<template>
    <header>
        <nav class="flex  bg-purple-900 text-white shadow-lg text-lg justify-between px-4">
            <NuxtLink to="/">Home</NuxtLink>
            <NuxtLink to="/about">About</NuxtLink>
            <NuxtLink to="/iphone">Iphones</NuxtLink>
            <NuxtLink to="/profile">Profile</NuxtLink> 
            <p>Cart ({{cart.length}})</p>
        </nav>
    </header> 
</template>


<!--
     we have a composable called useCart in the state.js file
     which we can call below
-->
<script setup>
    const cart = useCart();

    // just checking to see length value
    console.log(cart.value.length);

</script>