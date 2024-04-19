<template>
 <h2> User Component </h2>
 <div>
    <h2>{{ data.name }}</h2>
    <h2>{{ data.email }}</h2>
    <button v-on:click="getData(data.name)"> Click me</button>
 </div>
</template>
<script>
 export default {
    name : 'UserComp',
    props:{
        data:Object,
        getData:Function
    },
   /* methods:{
        getData(){
            alert("Hello")
        }
    }*/
 }
</script>