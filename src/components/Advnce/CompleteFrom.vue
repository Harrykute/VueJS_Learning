<template>
<h1> Complete Form Comp </h1>
<h2>{{ form }}</h2>
<ul>
    <li v-for="item in error" v-bind:key="item"> 
    {{ item }} NOt Valid</li>
</ul>


<form>
    <input type="text" id="email" placeholder="email" v-model="form.email" />
    <input type="password" id="password" placeholder="password" v-model="form.password" />
    <br />
    <label for="Country"> Country:</label>
    <select v-model="form.country" >
        <option>India</option>
        <option> China</option>
        <option>USA</option>
    </select>
    <br />
    <h3> Technology </h3>
    <label>Java : </label>
    <input type="checkbox" value="java" name="technology" v-model="form.technology"/>
    <br/> <br />
    <label>PHP: </label>
    <input type="checkbox" value="PHP" name="technology" v-model="form.technology"/>
    <br/> <br />
    <lable> .Net </lable>
    <input type="checkbox" value=".Net" name="technology" v-model="form.technology"/>1
    <br /> <br />

    <h3> Gender </h3>
    <label> Male </label>
    <input type="radio" value="male" name="gender" v-model="form.gender"/>
    <br/>
    <label> Female </label>
    <input type="radio" value="female" name="gender" v-model="form.gender"/>
    <br/> <br />

    <button v-on:click.prevent="login">Submit</button>
</form>
</template>

    
<script>
export default {
    name: 'CompleteFrom',
    data() {
        return {
            form: {
                email: '',
                password: '',
                country:'',
                technology:[],
                gender:''
            }, // after the completion of Form then work with error define in data
            error: [],
        }
    },
    methods: {
    
        login() {
            this.error = [];
             for(const item in this.form){
               
                if(this.form[item] === "" || this.form[item].length === 0){
                   this.error.push(item);
                }

                if(this.error.length === 0){
                    alert("Data is Submitted Succesfully ")
                }
             }

            //console.log("Email : " + this.form.email + " Password : " + this.form.password)
            console.warn(this.form , this.error)
        }
    }
}
</script>
