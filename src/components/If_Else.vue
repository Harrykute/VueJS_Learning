<template>
    <h1 v-if="show">If Condition</h1>
    <h1 v-else> Else condition</h1>
    <Button v-on:click="show=false">Click me For Toogle</Button>
</template>

<script>
        export default {
            name : "If_Else" ,
            data(){
                return {
                    show : true
                }
            }
        }
</script>