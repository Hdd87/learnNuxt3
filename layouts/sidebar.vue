<!-- this is another layout to be used inside the profile page  -->

<template>
    <main class="flex bg-teal-300">

        <article class="flex-col bg-slate-400 text-white font-bold">
            <NuxtLink to="/"><p> Home </p></NuxtLink>
            <NuxtLink to="/about"><p> About </p></NuxtLink>    
        </article>
    
    <section>
        <slot></slot>
    </section>
    


    </main>
</template>

<style>
/* add more styling later  */
    .sidebar {
        display: flex;
        flex-direction: column;
        background-color: aqua;
        
    }
    .container {
        display: flex;
        /* flex-direction: column; */
        background-color: blanchedalmond;
    }
</style>