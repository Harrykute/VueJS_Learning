<template> 
   <h1> Slot Parent Component </h1>
   <!-- Using <slot> tag in child component it will add tag using parent parent component-->
   <SlotChildComp> <h1>Adding h1 tag  </h1></SlotChildComp>
   <!-- We can also use default tags for add tag-->
  <SlotChildComp/>
 </template>
 <script>
 import SlotChildComp from './SlotChildComp.vue';
  export default {
    name: 'SlotParentComp',   
    components: {
      SlotChildComp
    }
  }
</script>