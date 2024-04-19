
<template> 
<h2> Student Name Is : {{ name }} </h2>
</template>

<script>
export default {
    name: 'StudentComp',
    props: {
        name:String
    }
}
</script>