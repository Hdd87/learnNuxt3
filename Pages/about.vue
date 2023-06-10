<template>
    <header>
        <nav>
            <ul>
                <li><NuxtLink to="/">Home</NuxtLink></li>
            </ul>
        </nav>
    </header>
    <h2>
        About page!
    </h2>

    <!-- use the navigateTo() method -->

    <button @click="moveTo">Home</button>

</template>

<script setup>
    function moveTo(){
        navigateTo("/")
    }
</script>