<template>
<h1> Get Check Box And Radio Button value </h1>
 <label>Java</label>
 <input type="checkbox" value="java" id="java" v-model="technology"/>

 <lable>PHP </lable>
 <input type="checkbox" value="php" id="php" v-model="technology"/>

 <label>Node</label>
 <input type="checkbox" value="node" id="node" v-model="technology"/>

 <br/> <br/>

 <label>Who I am</label>
 <label> Student </label>
 <input type="radio" value="student" v-model="who" id="student"/>

  <label> Developer</label>
  <input type="radio" value="developer" v-model="who" id="developer"/>

  <br/> <br/>

  <h4> Selected Technology : {{ technology }}</h4>
  <h4> I am : {{ who }}</h4>
</template>
   
<script>

export default {
    name : 'GetCheckAndRe',
    data() {
        return {
            technology : [],
            who : null
        }
    }
}

</script>