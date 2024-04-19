<template>
<h1> {{name2}}</h1>
<h1>{{ userName }}</h1>
<button v-on:click="getData()"> Get Data </button>
</template>

<script>

export default {
    name: 'ChildComp',
    props: {
        name2: String,
        getData: Function,
        user: Object
    }

}
</script>
