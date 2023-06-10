<!-- we will create another counter 2 with the options API ie only script-->

<template>
    <button>Increment</button>
    <p> {{ count }}</p>
    <button>Decrement</button>
</template>

<script>

export default {
    data(){
        return {
            count:0,
        }
    }, 
    methods:{
        increment(){
            this.count++;
        }, 
        decrement(){
            this.count--;
        },
    },
}

</script>

<!-- so this does not work in the app.vue -->
<!-- we are missing some info how to make this work  -->
<!-- we probably have to import this in the app.vue -->