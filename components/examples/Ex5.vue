<!-- 
    in this example we have 2 <a> tags
    which contain a function view()
    when we click the "Home" link we call the view() with param home
    then the page.value = home
    which renders the <HomeWelcome /> component

    the <Counter /> is rendered the same way 

    the page value is set to "home" at the start

    add the Lazy prefix to load component only when needed

 -->


<template>
    <a href="#" @click = "view('home')"><b>Home</b></a>
    <br/>
    <a href="#" @click = "view('counter')"><b>Counter</b></a>

    <LazyHomeWelcome v-if = "page === 'home'" />

    <LazyCounter v-if="page === 'counter'" />

</template>

<script setup>

const page = ref("home");

function view(name){
    page.value = name;
}
</script>