<template>
 <h1> Multiple Slot Parent Component </h1>
<MultipleSlotChildComp/>
<MultipleSlotChildComp>
<template v-slot:header><h1> Peter </h1></template>
 <template v-slot:main> <p> A Vue js product</p> </template>
 <template v-slot:footer> <button> Buy Now</button> </template>
</MultipleSlotChildComp>
 

</template>

<script>
import MultipleSlotChildComp from './MultipleSlotChildComp.vue';
       export default {
        name: 'MultipleSlotParentComp',
        components: {
            MultipleSlotChildComp
        }
       }
</script>