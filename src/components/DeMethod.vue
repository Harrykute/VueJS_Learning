<template>
<h1>De Method </h1>
<p> Name : {{ getName() }}</p>
<p> Name 2 : {{ getName2("Peter") }}</p>
<p> Data  Name : {{ getData().name }}</p> <!-- Accessing data from script using Methods -->
<p> Data Email : {{ getData().email }}</p>
<p> Data Email2 : {{ getData().email2 }}</p>
</template>
<script>

export default { 
    name : 'DeMethod',
    data(){
       return {
         email : "Harish@gmail.com"
       }  
    },
    methods : {
         getName(){
            return "Harish"
         },
         getName2(name){
           return name
         },
         getData(){
            return {
                name : 'anil',
                email : 'anil@gmail.com',
                //you can use this keyword also here it will fetch the data from
                // data() property 
                 email2 : this.email // this email comes from data() property
            }
         }
    }
}
</script>