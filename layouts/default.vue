<!-- default layout for this project -->

<!-- add the nav bars and the buttons here  -->

<template>
    <header>
        <nav class="bg-purple-400 text-white">
            <ul>
                <li><NuxtLink to="/">Home</NuxtLink></li>
                <li><NuxtLink to="/about">About</NuxtLink></li>
                <li><NuxtLink to="/profile">Profile</NuxtLink></li>
                <li><NuxtLink to="/iphone-[name]">Iphone</NuxtLink></li>
            </ul>
        </nav>
    </header> 

    <!-- use slot to add the content of the page -->
    <slot></slot>

    <div class="bg-blue-300 text-white space-x-4">
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
