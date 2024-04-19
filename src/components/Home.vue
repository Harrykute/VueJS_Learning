<template>
      <h1> Home component</h1>
      <!-- --><h1>Home Component {{ 10+10 }}</h1> <!-- It is interpolation in {{ Expression}}-->
      <h2>Home component {{ "Harish".length }}</h2>  <!-- It will print home componenet and length of harish string -->
      <!-- Using from Script -->
      <h3>Home component : Email = {{ email }}</h3>
      <h4>Home Component : Name = {{ getName() }}</h4> <!--Using function from script -->
      <h5> Home component : Company Name : {{ getName2("MKCL") }}</h5>
      <!-- Assigning value in interpolation -->
      <!-- it will override the value-->
      <h5>Home component : Salary : {{ salary = 8888 }} </h5>
  </template>
  
  <script>
  export default {
    name: 'HelloWord',
     data(){
      return{
        email : 'harish@gmail.com',
         getName : function(){
          return "Harish Kute"
        },
        //you can use paramterized function
        getName2 : function(name){
           return name
         },
         salary : 100000000000
      }
     }       
  }
  </script>
    
 
  <style>
  
  </style>