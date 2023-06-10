<!-- default layout for this project -->

<!-- add the nav bars and the buttons here  -->

<template>
    <header>
        <nav class="flex  bg-purple-400 text-white shadow-lg text-lg justify-between px-4">
            <NuxtLink to="/">Home</NuxtLink>
            <NuxtLink to="/about">About</NuxtLink>
            <NuxtLink to="/iphone">Iphones</NuxtLink>
            <NuxtLink to="/profile">Profile</NuxtLink>
            
        </nav>
    </header> 

    <!-- use slot to add the content of the page -->
    <slot></slot>

    <div class="bg-blue-300 text-white justify-between">
        <button @click="home">Home</button>
        <button @click="about">About</button>
        <button @click="profile">Profile</button>
    </div>
</template>

<script setup>
//  use the navigateTo() method 
    function about(){
        navigateTo("/about")
    }
    function home(){
        navigateTo("/")
    }
    function profile(){
        navigateTo("/profile")
    }

</script>
