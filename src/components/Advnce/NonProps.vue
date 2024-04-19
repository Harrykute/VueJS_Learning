<template>
<h1>Non Props Data </h1>
<User3 data="some data" id="cmp"/> <!-- When You pass this id it will reflect to the as attribute for div -->
</template>

<script>
import User3 from './User3.vue';
export default {
    name: 'NonPropsData',
    components: {
        User3
    }, 
}
</script>
