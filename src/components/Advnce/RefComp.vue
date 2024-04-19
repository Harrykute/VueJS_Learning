<template>
<h1> Ref In Vue Js </h1>
<input type="text" ref="input"/> <!-- This ref get all control so you can add style , or get and set value-->
<button v-on:click="getData()">Click me</button>
</template>
<script>
export default {
    name: 'RefInVueJs',
    methods: {
        getData(){
           // console.warn("-------");
           this.$refs.input.focus(); // after the click it focused to the input eg. cursor will blink 
           let val =this.$refs.input.value; // it will take value from input 
           console.warn(val);
           // now we can add style also 
           this.$refs.input.style.color="Red"; // it will change the color input field 
           this.$refs.input.style.backgroundColor="Yellow"; // it will change the background color input field 
        }
    }
}
</script>