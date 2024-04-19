<template>
<h1> User Resuse Component</h1>
<ul>
    <li v-for="item in users" :key="item.name">
     <!--{{ item.name }}-->
     <User :data="item" :getData = "getData"/> 
    </li>
</ul>
<User/>
</template>

<script>
import User from './User.vue';

export default {
  name: "UserParentComp",
  components:{
    User
  },
  methods:{
        getData(name){
            alert(name)
        }
    },
  data(){
    return{
        users:[
            {name:'anil' , email:'anil@test.com'},
            {name:'sam',email:'sam@test.com'},
            {name:'harish', email:'harish@gmail.com'},
            {name:'bruce' ,email:'bruce@gmail.com'} 
        ]
    }
  }
}
</script>

<style scoped></style>