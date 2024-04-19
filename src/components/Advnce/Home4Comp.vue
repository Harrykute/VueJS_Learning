<template>
    <h1> Parent Component </h1>
<h2> Send Data Child to parent in Vue js</h2>
<User2 :getUser="getUserName"/> <!-- Now in child component we have to create props property (User2Comp )-->
<h2>{{ childUser }}</h2> <!-- now it will print here after the button clicked-->
</template>

<script>
import User2 from './User2.vue';
export default {
    name: 'User2Comp',
    data(){
        return{
            childUser:""
        }
    },
    components: {
        User2
    },
    //Now We have to create function in parent component for pass data 
    methods: {
        getUserName(name){
          //  alert(name); // after creation of this we to pass to the child component <User :getUser="getUserName"
           this.childUser=name
        }
    }
}
</script>
