<template>
    <h2> User2 Component </h2>
    <button v-on:click="getUser(userName)">Send User Name </button>
</template>
<script>
export default {
    name: 'User2Comp',
    data() { // first created this in child Component 
        return {
            userName: "peter" // now this data should go in parent component 
        }
    },
    props:{
             getUser: Function,
    }
    
    }
</script>