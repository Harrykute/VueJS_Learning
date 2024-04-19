<template>
  <h1> Get Input Field Value </h1>
  <label for="Username">Username</label>
  <input type="text" placeholder="Enter UserName" v-model="username"/>
  <br/>
  <br/>
  <label>password</label>
  <input type="password" placeholder="Password" v-model="password"/>
  <button v-on:click="getData()">Click Me for data </button>
</template>

<script>
  export default {
    name : 'GetInputField',
    data(){
        return{
            username : null,
            password : null,
        }
    },
    methods : {
        getData(){
            console.warn("User Name : " , this.username ," password" , this.password); 
        }
    }
  }
</script>