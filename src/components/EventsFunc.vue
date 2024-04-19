<template>
    <div> 

    <h1> Events </h1>
        <button v-on:click="getData('Hello harish Thank you for click')">Click On Me </button>
         <button v-on:dblclick="getData('Hii Harish I came after double click')">Click Double to see Message</button>
         <button v-on:click="getConsole()">Get warn </button>
        </div>
        <div>
            <Button v-on:click = "getCount()">Increase Count</Button>
            <h1> Count : {{ count }}</h1>
        </div>
</template>

<script>
       
        export default {
            name : "EventsFunc",
            data(){
                return {
                    count : 0
                }
            },
            methods : {
                   getData(data){
                          alert(data);
                   },
                   getConsole(){
                    console.warn("I am From getConsole function")
                   },
                   getCount(){
                       return this.count++;
                   }
            }
        }
</script>