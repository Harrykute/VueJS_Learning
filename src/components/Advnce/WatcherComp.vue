<template> 
   <h1> Watcher Component </h1>
   <h2> {{ count }}</h2>
   <button v-on:click="count=count+1"> + </button>
   <button v-on:click="count=count-1"> - </button>
</template>
<script>
  export default {
    name: 'WatcherComp',
    data(){
        return {
            count: 0 
        }
    },
    watch: {
        // first we have created this for normal use means increment and decrement
        // Now we can some function to it 
        count(val,prev){
            // but only using if there is increasing automatically 
             if(val>5 && val>prev){
               alert("Value is greater than 5");
               this.count=0; 
             }
        }
    }
  }
</script>