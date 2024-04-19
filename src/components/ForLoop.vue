<template>
<h1> For Loop in Vue JS</h1> 
<ul>
    <li v-for="item in technology" :key="item">
    {{ item }}</li>
</ul>
<br/>
<br/>
<ul>
    <li v-for="item in user" :key="item.age"> Name is : {{ item.name }} Age is : {{ item.age }}</li>
</ul>
</template>
<script>
  export default {
    name : 'ForLoop',
    data(){
        return {
            technology : ['java','php','node','html'],
            user: [{
                name: 'Abhishek',
                age: 25,
            },
            {
                name: 'Aditya',
                age: 22,
            }]
        }
    }
  }


</script>
