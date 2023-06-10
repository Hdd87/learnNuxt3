<!-- default layout for this project -->

<!-- add the nav bars and the buttons here  -->

<template>
    <header>
        <nav>
            <ul>
                <li><NuxtLink to="/">Home</NuxtLink></li>
                <li><NuxtLink to="/about">About</NuxtLink></li>
                <li><NuxtLink to="/profile">Profile</NuxtLink></li>
            </ul>
        </nav>
    </header> 

    <slot></slot>

    <button @click="home">Home</button>
    <button @click="about">About</button>
    <button @click="profile">Profile</button>

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
