<template>
<h1> Simple Form Comp </h1>
<form > 
    <input type="text" id="email" placeholder="email" v-model="form.email" />
    <input type="password" id="password" placeholder="password" v-model="form.password" />
    <!-- <button type="submit">Submit</button> --> 
    <!-- .prevent method is used to stop the page refresh 
        here is happning when i clicked the submit the page is refreshing so i used the .prevent -->
    <button v-on:click.prevent="login">Submit</button>
</form>
</template>

<script>
export default {
    name: 'simpleForm',
    data() {
        return {
            form: {
            email:'',
            password:''
        }
        }
    },
    methods: {
        login(){
           console.log("Email : " + this.form.email + " Password : "+ this.form.password)
        }
    }
}
</script>
