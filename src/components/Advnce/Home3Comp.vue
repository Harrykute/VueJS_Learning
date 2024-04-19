<template>
    <h1>Props in Vue js 3</h1>
    <Student :name="name"/>
    <Teacher name="MK Jadhav"/>
</template>
<script>
import Student from './Student.vue';
import Teacher from './Teacher.vue';
export default {
    name: 'Home3Comp',
    data(){
         return{
            name: "Kute"
         }
    },
    components:{
        Student,
        Teacher
    }
}
</script>