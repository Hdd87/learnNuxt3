<!-- default layout for this project -->

<!-- add the nav bars and the buttons here  -->

<template>
    <header>
        <nav>
            <ul>
                <li><NuxtLink to="/about">About</NuxtLink></li>
                <li><NuxtLink to="/">Home</NuxtLink></li>
            </ul>
        </nav>
    </header> 

    <slot></slot>

    <button @click="about">About</button>
    <button @click="home">Home</button>

</template>

<script setup>
//  use the navigateTo() method 
    function about(){
        navigateTo("/about")
    }
    function home(){
        navigateTo("/")
    }
</script>
