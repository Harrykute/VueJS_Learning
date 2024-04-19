<template>
    <h1> Form Modifiers</h1>
    <!-- <input type="text" v-model.lazy="data"> -->
    <input type="text" v-model.trim="data">
    <h2>Data is : {{ data }}</h2>
</template>
<script>
    export default {
        name: 'FormModifiers',
        data(){
            return{
                data: '',
            }
        },
        methods: {
            
        }


    }
</script>