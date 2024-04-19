<template>
    <h1> Html Binding </h1>
<h1>{{ text }} </h1>
<div v-html="tag"> </div>
<div v-html="tag2"> </div> 
</template>

<script>
export default {
     name:'HtmlBinding',
     data(){
        return{
            text:"Harish Kute From HTML Binding",
            tag:'<h2>This is a HTML Binding for h2 tag </h2>',
            tag2:'<h3> This is a HTML Binding for h3 tag </h3>'
        }
     }
}
</script>
