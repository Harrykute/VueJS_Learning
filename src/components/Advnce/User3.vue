<template>
<!-- <div> 
  <h3> Peter</h3>
  <h3> Bruce</h3>
  <h3> Anil</h3>  
  <h3>{{ data }} </h3>
</div>   -->

<!-- If you remove the div then id will not with any tag -->
<!-- If you want to bind this to tag then use v-bind="$attrs" -->

  <h3 v-bind="$attrs"> Peter</h3> <!-- It will add to the tag -->
  <h3> Bruce</h3>
  <h3> Anil</h3>  
  <h3>{{ data }} </h3>
     
</template>
<script>
  export default {
    name: 'User3Comp',
    props: {
        data:String
    }
  }
</script>