<template>
    <header>
        <nav>
            <ul>
                <li><NuxtLink to="/about">About</NuxtLink></li>
            </ul>
        </nav>
    </header>

    <h2>Index page !</h2>   

    <button @click="moveTo">About</button>

</template>

<script setup>
//  use the navigateTo() method 
    function moveTo(){
        navigateTo("/about")
    }
</script>
