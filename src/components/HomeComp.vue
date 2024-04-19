<template>
<h1> Home Component 2 for pass data</h1>
<h2> Pass data to child Component</h2>
<h3>Child Comp</h3>
<ChildComp name2='Harish Kute' :getData="getData" :user="user" />
</template>

<script>
import ChildComp from './ChildComp.vue';
export default {
    name: 'HomeComp',
    components: {
        ChildComp
    },
    data() {
        return {
            user: {
                username: 'Harish',
                age: 20
            }
        }
    },
    methods: {
        getData() {
            console.warn("Parent function called ");
        }
    }
}
</script>
