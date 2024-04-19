<template>
<h1> Computed Property </h1>
<h2>{{ (dollors*rupeeVal)-discount }}</h2>
<h2>{{ getResult }}</h2>
</template>

<script>
export default {
    name: "ComputedProp",
    data() {
        return {
            dollors: 100,
            rupeeVal: 70,
            discount: 10
        }
    },
    computed: {
        getResult() {
            return (this.dollors*this.rupeeVal)-this.discount;
        }
    }
}
</script>
